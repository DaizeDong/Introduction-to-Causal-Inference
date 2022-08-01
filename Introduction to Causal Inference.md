# Introduction to Causal Inference

This is a brief note on [Brady Neal](https://www.bradyneal.com/aboutme)'s online causal inference course. Contents are arranged by the course textbook. Some sections are slightly modified according to my personal comprehension to help understanding. *Last update on August 1st, 2022.*

**Course Website：** [Introduction to Causal Inference (bradyneal.com)](https://www.bradyneal.com/causal-inference-course)

**Textbook：** [Introduction_to_Causal_Inference-Dec17_2020-Neal](https://www.bradyneal.com/Introduction_to_Causal_Inference-Dec17_2020-Neal.pdf)





## 1 Motivation: Why You Might Care

### Association is Not Causation

**Association:** Statistical dependence between two subjects.

**Confounding Association:** The association facilitated by a confounder.





## 2 Potential Outcomes

### Fundamental Concepts

**Observed Outcome:**
$$
Y
$$
**Potential Outcome:** 
$$
Y(t)
$$
**Individual Treatment Effect (ITE) / Individual Causal Effect (ICE):** 
$$
\tau_i=Y_i(1)-Y_i(0)
$$
**Average Treatment Effect (ATE) / Average Causal Effect (ACE):** 
$$
\begin{aligned}
\tau&=\mathbb{E}\big[Y_i(1)-Y_i(0)\big]\\
&=\mathbb{E}\big[Y(1)-Y(0)\big]\\
&=\mathbb{E}\big[Y(1)\big]-\mathbb{E}\big[Y(0)\big]
\end{aligned}
$$
**Associational Difference:**
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





## 3 The Flow of Association and Causation in Graphs

### Bayesian Networks

#### Basic Assumptions

**Local Markov Assumption:** 

- Given its parents in the DAG (Directed Acyclic Graph), a node $X$ is independent of all its non-descendants.

With local Markov assumption, we can simplify the factor:

<img src="figs\3.6.png" style="zoom:50%;" />
$$
\begin{aligned}
P(x_1.x_2,x_3,x_4)&=P(x_1)P(x_2|x_1)P(x_3|x_2,x_1)P(x_4|x_3,x_2,x_1)\\
&=P(x_1)P(x_2|x_1)P(x_3|x_2,x_1)P(x_4|x_3)
\end{aligned}
$$
**Minimality Assumption:** 

1. Given its parents in the DAG, a node $X$ is independent of all its non-descendants. **(Local Markov Assumption)**
2. Adjacent nodes in the DAG are dependent.

The minimality assumption gives an additional constraint on the direction of independence.

<img src="figs\3.8.png" style="zoom:50%;" />
$$
\begin{aligned}
P(x,y)&=P(x)P(y|x)\\
&\ne P(y)P(x|y)
\end{aligned}
$$

#### Basic Blocks

We will study the association from three basic blocks in Bayesian networks.

<img src="figs\3.9.png" style="zoom:55%;" />

|                         Basic Block                          |             Association ($X_1$ and $X_3$)             |                            Proof                             |
| :----------------------------------------------------------: | :---------------------------------------------------: | :----------------------------------------------------------: |
|   <img src="figs\3.12.png" style="zoom:50%;" /><br/>Chain    |                       Dependent                       |                            ——————                            |
| <img src="figs\3.14.png" style="zoom:50%;" /><br />Conditioned Chain |            ***Conditionally Independent***            | $\begin{aligned}P(x_1,x_3|x_2)&=\dfrac{P(x_1,x_2,x_3)}{P(x_2)}\\&=\dfrac{P(x_1)P(x_2|x_1)P(x_3|x_2)}{P(x_2)}\\&=\dfrac{P(x_1,x_2)P(x_3|x_2)}{P(x_2)}\\&=P(x_1|x_2)P(x_3|x_2)\end{aligned}$ |
|   <img src="figs\3.13.png" style="zoom:50%;" /><br />Fork    |                       Dependent                       |                            ——————                            |
| <img src="figs\3.15.png" style="zoom:50%;" /><br />Conditioned Fork |            ***Conditionally Independent***            | $\begin{aligned}P(x_1,x_3|x_2)&=\dfrac{P(x_1,x_2,x_3)}{P(x_2)}\\&=\dfrac{P(x_1|x_2)P(x_2)P(x_3|x_2)}{P(x_2)}\\&=P(x_1|x_2)P(x_3|x_2)\end{aligned}$ |
| <img src="figs\3.16.png" style="zoom:50%;" /><br />Immorality | ***Independent***<br />($X_2$ is called the collider) | $\begin{aligned}P(x_1,x_3)&=\sum_{x_2}P(x_1,x_2,x_3)\\&=\sum_{x_2}P(x_1)P(x_3)P(x_2|x_1,x_3)\\&=P(x_1)P(x_3)\sum_{x_2}P(x_2|x_1,x_3)\\&=P(x_1)P(x_3)\end{aligned}$ |
| <img src="figs\3.17.png" style="zoom:50%;" /><br />Conditioned Immorality |                Conditionally Dependent                |                            ——————                            |

#### D-separation & Markov Assumption

**Blocked Path:** A path $X\rightarrow\dots\rightarrow Y$ is blocked by a conditioning set $Z$ (can be empty) if either of the following is true:

1. Along the path, there is a chain $\dots\rightarrow W\rightarrow\dots$ or a fork $\dots\leftarrow W\rightarrow\dots$ , where  $W\in Z$.

2. Along the path, there is a collider $\dots\rightarrow W\leftarrow\dots$ , where $W,\text{de}(W)\notin Z$,

   in which $\text{de}(\cdot)$ means descendants.

**D-separation:** Given a set of nodes $Z$, two nodes $X,Y$.

- $X,Y$ are d-separated by $Z$ if all paths between $X,Y$ are blocked by $Z$.

**(Global) Markov Assumption:** <!--Note: This section is a little ambiguous-->

- Given: $P$ is Markov with respect to $G$.

  If $X,Y$ are d-separated in $G$ conditioned on $Z$, then $X,Y$ are independent in $P$ conditioned on $Z$.
  $$
  X⫫_GY\ |\ Z\Longrightarrow X⫫_PY\ |\ Z
  $$



### Causal Graphs

**Cause:** A variable $X$ is said to be a cause of a variable $Y$, if $Y$ can change in response to changes in $X$.

**(Strict) Causal Edges Assumption:** In a directed graph, *every* parent is a direct cause of all its children.

**(Non-strict) Causal Edges Assumption:** In a directed graph, *some* parent is a direct cause of all its children.

<img src="figs\3.20.png" style="zoom:60%;" />

Causation is a sub-category of association. Our objective is to isolate causation from association.

**D-separation Implies Association is Causation:** Only association conducted from a chain is the causation.

<img src="figs\3.a.png" style="zoom:60%;" />

<img src="figs\3.21.png" style="zoom:70%;" />



## 4 Causal Models



















