# Introduction to Causal Inference

This is a brief note on [Brady Neal]([Brady Neal - About Me](https://www.bradyneal.com/aboutme))'s online causal inference course. Contents are arranged by the course textbook. Some sections are slightly modified according to my personal comprehension to help understanding. *Last update on July 31th, 2022.*

**Course Website：** [Introduction to Causal Inference (bradyneal.com)](https://www.bradyneal.com/causal-inference-course)

**Textbook：** [Introduction_to_Causal_Inference-Dec17_2020-Neal](https://www.bradyneal.com/Introduction_to_Causal_Inference-Dec17_2020-Neal.pdf)



## 1 Motivation: Why You Might Care

### Association is Not Causation

**Association:** Statistical dependence between two subjects.

**Confounding Association:** The association facilitated by a confounder.



## 2 Potential Outcomes

### Fundamental Concepts

Observed Outcome:
$$
Y
$$
Potential Outcome: 
$$
Y(t)
$$
Individual Treatment Effect (ITE) / Individual Causal Effect (ICE): 
$$
\tau_i=Y_i(1)-Y_i(0)
$$
Average Treatment Effect (ATE) / Average Causal Effect (ACE): 
$$
\begin{aligned}
\tau&=\mathbb{E}\big[Y_i(1)-Y_i(0)\big]\\
&=\mathbb{E}\big[Y(1)-Y(0)\big]\\
&=\mathbb{E}\big[Y(1)\big]-\mathbb{E}\big[Y(0)\big]
\end{aligned}
$$
Associational Difference:

$$
\mathbb{E}\big[Y|T=1\big]-\mathbb{E}\big[Y|T=0\big]
$$


### Fundamental Problem of Causal Inference

An individual $i$ cannot observe two potential outcomes $Y_i(1),Y_i(0)$ at the same time. i.e., $\tau_i$ cannot be observed.

**Factual:** The observed outcome.

**Counterfactual:** Outcomes cannot be observed.



### Getting Around the Fundamental Problem (5 Assumptions)

#### Ignorability / Exchangeability

$$
\big(Y(1),Y(0)\big)⫫T
$$

<img src="figs\2.2.png" style="zoom:53%;" />

Under exchangeability assumption, we have:
$$
\begin{aligned}
&\mathbb{E}\big[Y(0)|T=0\big]=\mathbb{E}\big[Y(0)|T=1\big]=\mathbb{E}\big[Y(0)\big]\\
&\mathbb{E}\big[Y(1)|T=0\big]=\mathbb{E}\big[Y(1)|T=1\big]=\mathbb{E}\big[Y(1)\big]
\end{aligned}
$$
So that:
$$
\begin{aligned}
\tau&=\mathbb{E}\big[Y(1)-Y(0)\big]\\
&=\mathbb{E}\big[Y(1)\big]-\mathbb{E}\big[Y(0)\big]\\
&=\mathbb{E}\big[Y(1)|T=1\big]-\mathbb{E}\big[Y(0)|T=0\big]
\end{aligned}
$$

#### Conditional Exchangeability / Unconfoundedness

$$
\big(Y(1),Y(0)\big)⫫T|X
$$

<img src="figs\2.4.png" style="zoom:61%;" />

**Motivation:** In observational data, it is unrealistic to assume that the treatment groups are exchangeable.

Under conditional exchangeability assumption, we have:
$$
\begin{aligned}
&\mathbb{E}\big[Y(0)|T=0,X\big]=\mathbb{E}\big[Y(0)|T=1,X\big]=\mathbb{E}\big[Y(0)|X\big]\\
&\mathbb{E}\big[Y(1)|T=0,X\big]=\mathbb{E}\big[Y(1)|T=1,X\big]=\mathbb{E}\big[Y(1)|X\big]
\end{aligned}
$$
So that:
$$
\begin{aligned}
\tau&=\mathbb{E}_X\mathbb{E}\big[Y(1)-Y(0)|X\big]\\
&=\mathbb{E}_X\Big[\mathbb{E}\big[Y(1)|X\big]-\mathbb{E}\big[Y(0)|X\big]\Big]\\
&=\mathbb{E}_X\Big[\mathbb{E}\big[Y(1)|T=1,X\big]-\mathbb{E}\big[Y(0)|T=0,X\big]\Big]
\end{aligned}
$$

#### Positivity / Overlap / Common Support

$$
0<P(T=t|X=x)<1
$$

This excludes some invalid circumstances where $x$ is not associated with $t$.

#### No Interference

$$
Y_i(t_1,t_2,\dots,t_n)=Y_i(t_i)
$$

No interference means that my outcome $Y_i$ is unaffected by anyone else’s treatment $t_k,\ k\in[1,n]-\{i\}$.

Rather, my outcome $Y_i$ is only a function of my own treatment $t_i$.

#### Consistency

$$
\begin{aligned}
&T=t\ \Longrightarrow\ Y=Y(t)\\
&\text{i.e.}\quad Y=Y(T)
\end{aligned}
$$

**Identifiability:** A causal quantity $\mathbb{E}\big[Y(t)\big]$ is identifiable if we can compute it from a purely statistical quantity $\mathbb{E}\big[Y|t\big]$.

Under consistency assumption, we can prove identifiability:

$$
\begin{aligned}
\tau&=\mathbb{E}\big[Y(1)-Y(0)\big]\\
&=\mathbb{E}\big[Y(1)\big]-\mathbb{E}\big[Y(0)\big]\\
&=\mathbb{E}\big[Y(1)|T=1\big]-\mathbb{E}\big[Y(0)|T=0\big]\quad\text{(Exchangeability)}\\
&=\mathbb{E}\big[Y|T=1\big]-\mathbb{E}\big[Y|T=0\big]\quad\text{(Consistency)}\\
\\
\tau&=\mathbb{E}_X\mathbb{E}\big[Y(1)-Y(0)|X\big]\\
&=\mathbb{E}_X\Big[\mathbb{E}\big[Y(1)|X\big]-\mathbb{E}\big[Y(0)|X\big]\Big]\\
&=\mathbb{E}_X\Big[\mathbb{E}\big[Y(1)|T=1,X\big]-\mathbb{E}\big[Y(0)|T=0,X\big]\Big]\quad\text{(Conditional Exchangeability \& Positivity)}\\
&=\mathbb{E}_X\Big[\mathbb{E}\big[Y|T=1,X\big]-\mathbb{E}\big[Y|T=0,X\big]\Big]\quad\text{(Consistency)}
\end{aligned}
$$

#### Stable Unit-treatment Value Assumption (SUTVA)

A combination of consistency and no interference.



### Fancy Statistics Terminology Defancified

**Estimand:** The quantity that we want to estimate.

**Estimate (noun):** An approximation of some estimand using data.

**Estimator:** A function that maps a dataset to an estimate of the estimand.

**Estimate (verb):**  Feed data into an estimator.

**Estimation:** The process of an estimate.

#### Causal Estimand & Statistical Estimand

<img src="figs\2.5.png" style="zoom:70%;" />



















