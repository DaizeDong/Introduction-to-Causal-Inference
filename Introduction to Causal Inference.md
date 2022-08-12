# Introduction to Causal Inference

This is a brief note on [Brady Neal](https://www.bradyneal.com/aboutme)'s online causal inference course. Contents are arranged by the course textbook. Some sections are slightly modified according to my personal comprehension to help understanding. *Last update on August 1st, 2022.*

**Course Website：** [Introduction to Causal Inference (bradyneal.com)](https://www.bradyneal.com/causal-inference-course)

**Videos:** [Intro and Outline of A Brief Introduction to Causal Inference - YouTube](https://www.youtube.com/watch?v=CfzO4IEMVUk&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0)

**Textbook：** [Introduction_to_Causal_Inference-Dec17_2020-Neal](https://www.bradyneal.com/Introduction_to_Causal_Inference-Dec17_2020-Neal.pdf)

| Week         | Topics                                                       | Lecture                                                      | Readings                        | Reading Group Paper                                          |
| :----------- | :----------------------------------------------------------- | :----------------------------------------------------------- | :------------------------------ | :----------------------------------------------------------- |
| August 31    | Motivation Course Preview Course Information                 | [Video](https://www.youtube.com/watch?v=CfzO4IEMVUk&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=1) [Slides](https://www.bradyneal.com/slides/1 - A Brief Introduction to Causal Inference.pdf) [Info](https://www.youtube.com/watch?v=xj-tzrm5Src&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=6) | Chapter 1 of ICI                | None                                                         |
| September 7  | Potential Outcomes A Complete Example with Estimation        | [Video](https://www.youtube.com/watch?v=q8x9aetyok0&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=8) [Slides](https://www.bradyneal.com/slides/2 - Potential Outcomes.pdf) | Chapter 2 of ICI                | [Does obesity shorten life? The importance of well-defined interventions to answer causal questions (Hernán & Taubman, 2008)](https://www.nature.com/articles/ijo200882) |
| September 14 | Graphical Models                                             | [Video](https://www.youtube.com/watch?v=Go4EkHN_PcA&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=19) [Slides](https://www.bradyneal.com/slides/3 - The Flow of Association and Causation in Graphs.pdf) | Chapter 3 of ICI                | [Does Obesity Shorten Life? Or is it the Soda? On Non-manipulable Causes (Pearl, 2018)](https://ftp.cs.ucla.edu/pub/stat_ser/r483-reprint.pdf) |
| September 21 | Backdoor Adjustment Structural Causal Models                 | [Video](https://www.youtube.com/watch?v=dB8r4Afmobo&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=28) [Slides](https://www.bradyneal.com/slides/4 - Causal Models.pdf) | Chapter 4 of ICI                | [Single World Intervention Graphs: A Primer (Richardson & Robins, 2013)](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.644.1881&rep=rep1&type=pdf) |
| September 28 | Randomized Experiments Frontdoor Adjustment *do*-calculus Graph-Based Identification | [Video](https://www.youtube.com/watch?v=z91LnTDyhtI&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=37) [Slides](https://www.bradyneal.com/slides/5 - Identification.pdf) | Chapters 5-6 of ICI             | [On Pearl’s Hierarchy and the Foundations of Causal Inference (Bareinboim et al., 2020)](https://causalai.net/r60.pdf) |
| October 5    | Estimation [Susan Athey](https://athey.people.stanford.edu/) Guest Talk - Estimating Heterogeneous Treatment Effects (Oct 8th at 3 - 4 pm EDT) | [Video](https://www.youtube.com/watch?v=YzcOYU-s2t4&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=42) [Slides](https://www.bradyneal.com/slides/6 - Estimation.pdf) [Guest Talk](https://www.youtube.com/watch?v=oZoizsX3bts&list=PLoazKTcS0RzZ1SUgeOgc6SWt51gfT80N0&index=7) | Chapter 7 of ICI                | [Adapting Neural Networks for the Estimation of Treatment Effects (Shi, Blei, Veitch, 2019)](https://arxiv.org/abs/1906.02120) |
| October 12   | Unobserved Confounding, Bounds, and Sensitivity Analysis     | [Video](https://www.youtube.com/watch?v=IXNMYqUsBBQ&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=47) [Slides](https://www.bradyneal.com/slides/7 - Unobserved Confounding.pdf) | Chapter 8 of ICI                | [Sense and Sensitivity Analysis: Simple Post-Hoc Analysis of Bias Due to Unobserved Confounding (Veitch & Zaveri, 2020)](https://arxiv.org/abs/2003.01747) |
| October 19   | Instrumental Variables                                       | [Video](https://www.youtube.com/watch?v=Mco16tUSA-U&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=53) [Slides](https://www.bradyneal.com/slides/8 - Instrumental Variables.pdf) | Chapter 9 of ICI                | [Deep IV: A Flexible Approach for Counterfactual Prediction (Hartford et al., 2017)](http://proceedings.mlr.press/v70/hartford17a.html) |
| October 26   | Difference-in-Differences [Alberto Abadie](http://economics.mit.edu/faculty/abadie) Guest Talk - Synthetic Control (Oct 29th at 10 - 11 am EDT) | [Video](https://www.youtube.com/watch?v=tT8xLRS_cRQ&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=58) [Slides](https://www.bradyneal.com/slides/9 - Difference-in-Differences.pdf) [Guest Talk](https://www.youtube.com/watch?v=nKzNp-qpE-I&list=PLoazKTcS0RzZ1SUgeOgc6SWt51gfT80N0&index=11) | Chapter 10 of ICI               | [Regression Discontinuity Designs in Economics (Lee & Lemieux, 2010)](https://www.princeton.edu/~davidlee/wp/RDDEconomics.pdf) |
| November 2   | --- Break Week - No Lecture ---                              | None                                                         | Past Readings                   | None                                                         |
| November 9   | Causal Discovery from Observational Data [Jonas Peters](http://web.math.ku.dk/~peters/) Guest Talk (November 13 at 10 am EST) | [Video](https://www.youtube.com/watch?v=lVE-4deFe7c&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=62) [Slides](https://www.bradyneal.com/slides/10 - Causal Discovery from Observational Data.pdf) | Chapter 11 of ICI               | [Inferring causation from time series in Earth system sciences (Runge et al., 2019)](https://www.nature.com/articles/s41467-019-10105-3) |
| November 16  | Causal Discovery from Interventions                          | [Video](https://www.youtube.com/watch?v=de2ODel8F1k&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=69) [Slides](https://www.bradyneal.com/slides/11 - Causal Discovery from Interventions.pdf) | Chapter 12 of ICI (Coming soon) | [Permutation-based Causal Inference Algorithms with Interventions (Wang et al., 2017)](https://arxiv.org/abs/1705.10220) |
| November 23  | Transfer Learning Transportability                           | [Video](https://www.youtube.com/watch?v=JNq4oCV9C5k&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=77) [Slides](https://www.bradyneal.com/slides/12 - Transfer Learning and Transportability.pdf) | Chapter 13 of ICI (Coming soon) | [A causal framework for distribution generalization (Christiansen et al., 2020)](https://arxiv.org/abs/2006.07433) |
| November 30  | [Yoshua Bengio](https://yoshuabengio.org/profile/) Guest Talk - Causal Representation Learning (Dec 1st at 1 - 2:30 pm EST) | [Guest Talk](https://www.youtube.com/watch?v=rKZJ0TJWvTk&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=80) [Slides](https://www.bradyneal.com/slides/Yoshua_Bengio_Guest_Talk_Towards_Causal_Representation_Learning.pdf) | None                            | [Invariant Risk Minimization (Arjovsky et al., 2019)](https://arxiv.org/abs/1907.02893) |
| December 7   | Counterfactuals Mediation                                    | [Video](https://www.youtube.com/watch?v=f8PEpthLlN4&list=PLoazKTcS0Rzb6bb9L508cyJ1z-U9iWkA0&index=81) [Slides](https://www.bradyneal.com/slides/14 - Counterfactuals and Mediation.pdf) | Chapter 14 of ICI (Coming soon) | [Identifiability of Path-Specific Effects (Avin, Shpitser, & Pearl, 2005)](https://ftp.cs.ucla.edu/pub/stat_ser/r321-ijcai05.pdf) |





# 1 Motivation: Why You Might Care

> ***Distinguish association and causation.***

## 1.1 Association is Not Causation

**Association:** Statistical dependence between two subjects.

**Confounding Association:** The association facilitated by a confounder.





# 2 Potential Outcomes

> ***Estimate causation with conditions.***

## 2.1 Fundamental Concepts

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

## 2.2 Fundamental Problem of Causal Inference

An individual $i$ cannot observe two potential outcomes $Y_i(1),Y_i(0)$ at the same time. i.e., $\tau_i$ cannot be observed.

**Factual:** The observed outcome.

**Counterfactual:** Outcomes cannot be observed.

## 2.3 Getting Around the Fundamental Problem (5 Assumptions)

### Ignorability / Exchangeability

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

### Conditional Exchangeability / Unconfoundedness

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

### Positivity / Overlap / Common Support

$$
0<P(T=t|X=x)<1
$$

This excludes some invalid circumstances where $x$ is not associated with $t$.

### No Interference

$$
Y_i(t_1,t_2,\dots,t_n)=Y_i(t_i)
$$

No interference means that my outcome $Y_i$ is unaffected by anyone else’s treatment $t_k,\ k\in[1,n]-\{i\}$.

Rather, my outcome $Y_i$ is only a function of my own treatment $t_i$.

### Consistency

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

### Stable Unit-treatment Value Assumption (SUTVA)

A combination of consistency and no interference.

## 2.4 Fancy Statistics Terminology Defancified

**Estimand:** The quantity that we want to estimate.

**Estimate (noun):** An approximation of some estimand using data.

**Estimator:** A function that maps a dataset to an estimate of the estimand.

**Estimate (verb):**  Feed data into an estimator.

**Estimation:** The process of an estimate.

**Causal Estimand & Statistical Estimand:** 

<img src="figs\2.5.png" style="zoom:70%;" />

## 2.5 Example

Check the textbook for details.



# 3 The Flow of Association and Causation in Graphs

> ***Model causation with graphs.***

## 3.1 Bayesian Networks

### Basic Assumptions

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

### Basic Blocks

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

### d-separation & Markov Assumption

**Blocked Path:** A path $X\rightarrow\dots\rightarrow Y$ is blocked by a conditioning set $Z$ (can be empty) if either of the following is true:

1. Along the path, there is a chain $\dots\rightarrow W\rightarrow\dots$ or a fork $\dots\leftarrow W\rightarrow\dots$ , where  $W\in Z$.

2. Along the path, there is a collider $\dots\rightarrow W\leftarrow\dots$ , where $W,\text{de}(W)\notin Z$,

   in which $\text{de}(\cdot)$ means descendants.

**D-separation:** Given a set of nodes $Z$, two nodes $X,Y$.

- $X,Y$ are d-separated by $Z$ if all paths between $X,Y$ are blocked by $Z$.

**(Global) Markov Assumption:**

- Given: $P$ is Markov with respect to $G$. <!--P is a Markov Process-->

  If $X,Y$ are d-separated in $G$ conditioned on $Z$, then $X,Y$ are independent in $P$ conditioned on $Z$.
  $$
  X⫫_GY\ |\ Z\Longrightarrow X⫫_PY\ |\ Z
  $$

## 3.2 Causal Graphs

**Cause:** A variable $X$ is said to be a cause of a variable $Y$, if $Y$ can change in response to changes in $X$.

**(Strict) Causal Edges Assumption:** In a directed graph, *every* parent is a direct cause of all its children.

**(Non-strict) Causal Edges Assumption:** In a directed graph, *some* parent is a direct cause of all its children.

<img src="figs\3.20.png" style="zoom:60%;" />

Causation is a sub-category of association. Our objective is to isolate causation from association.

**d-separation Implies Association is Causation:** Only association conducted from a chain is the causation.

<img src="figs\3.a.png" style="zoom:60%;" />

<img src="figs\3.21.png" style="zoom:70%;" />





# 4 Causal Models

> ***Estimate causation with specified conditions.***

## 4.1 Fundamental Concepts

**do-operator:** $\text{do}(t)$ or $\text{do}(T=t)$ indicates the intervention on whole samples with $T=t$.

**Observational Distribution:**
$$
P(Y)
$$
**Interventional Distribution:**
$$
P\big(Y\ |\ \text{do}(t)\big)
$$
<img src="figs\4.2.png" style="zoom:60%;" />

**Statistical Estimand:** An estimand without do-operator.

**Causal Estimand:** An estimand with do-operator.

**Identifiable:** An interventional expression $Q$ is identifiable if it can be reduced to an observational expression (without do in it).

**Causal Mechanism:** The conditional distribution of $X_i$ given all of its causes:
$$
P(x_i\ |\ \text{pa}_i)
$$

**Sufficient Adjustment Set:** $W$ is a sufficient adjustment set if is satisfies:
$$
\mathbb{E}\big[Y(t)\ |\ W=w\big]=\mathbb{E}\big[Y\ |\ \text{do}(t),W=w\big]=\mathbb{E}\big[Y\ |\ t,w\big]
$$

## 4.2 Causal Bayesian Networks

### Modularity / Independent Mechanisms / Invariance

If we set a set of nodes $S$ to constants $c_i$ (intervention), then for all $i$, we have:

1. If $i\notin S$, then $P(x_i\ |\ \text{pa}_i)$ remains unchanged.
2. If $i\in S$, then $\begin{cases}P(x_i=c_i\ |\ \text{pa}_i)=1\quad(x_i\text{ is consistent with the intervention)}\\P(x_i\ne c_i\ |\ \text{pa}_i)=0\end{cases}$.

This indicates that the interventions are local, i.e., they only change the probabilities of intervened nodes.

### Manipulated Graph

The causal graph for interventional distributions is the graph with all of the edges to the intervened node(s) removed.

<img src="figs\4.4.png" style="zoom:60%;" />

### Truncated Factorization

Given a set of intervention nodes $S$, if $x$ is consistent with the intervention, then:
$$
P\big(x_1,\dots,x_n\ |\ \text{do}(S=s)\big)=\prod_{i\notin S}P(x_i\ |\ \text{pa}_i),
$$
otherwise, we have:
$$
P\big(x_1,\dots,x_n\ |\ \text{do}(S=s)\big)=0.
$$
This is an extended form of the regular factorization with with modularity applied. <!--easy to prove-->

## 4.3 The Backdoor Adjustment

### Backdoor Criterion

**Backdoor paths:** All non-causal association paths (forks and conditioned immoralities).

A set of variables $W$ satisfies the <u>backdoor criterion</u> relative to $T$ and $Y$ if the following are true:

1. $W$ blocks all backdoor paths from $T$ to $Y$.
2. $W$ does not contain any descendants of $T$.

Satisfying the backdoor criterion makes $W$ a <u>sufficient adjustment set</u>.

It also indicates that $T$ is the causation of $Y$ under condition $W$.

#### Why to Not Condition on Descendants of Treatment

1. We block the flow of causation from $T$ to $Y$.
2. We induce non-causal association between $T$ and $Y$.

<img src="figs\4.a.png" style="zoom:55%;" />

However, if we only condition on the descendants, we can still induce <u>collider bias</u>.

An example of **M-bias**:

<img src="figs\4.16.png" style="zoom:60%;" />

### Backdoor Adjustment

Given the modularity assumption that $W$ satisfies the backdoor criterion and positivity, we can identify the causal effect of $T$ on $Y$:
$$
P\big(y\ |\ \text{do}(t)\big)=\sum_wP\big(y\ |\ t,w\big)P\big(w\big)
$$
Proof of the <u>backdoor adjustment</u>:
$$
\begin{aligned}
P\big(y\ |\ \text{do}(t)\big)&=\sum_wP\big(y,w\ |\ \text{do}(t)\big)\\
&=\sum_wP\big(y\ |\ \text{do}(t),w\big)P\big(w\ |\ \text{do}(t)\big)\\
&=\sum_wP\big(y\ |\ t,w\big)P\big(w\ |\ \text{do}(t)\big)\quad\text{(T is the causation of Y under condition W)}\\
&=\sum_wP\big(y\ |\ t,w\big)P\big(w\big)\quad\text{(Modularity between W and T)}
\end{aligned}
$$

### Relation to d-separation

We can use the backdoor adjustment if $W$ <u>d-separates $T$ from $Y$</u> in the manipulated graph.

i.e., $Y\Longrightarrow T$ doesn't have any association path.

i.e., $T\Longrightarrow Y$ doesn't have any non-causation association path.

### Relation to Potential Outcomes

Here we have the interventional distribution:
$$
\begin{aligned}
\mathbb{E}\big[Y\ |\ \text{do}(T=t)\big]&=\sum_w\mathbb{E}\big(y\ |\ t,w\big)P\big(w\big)\\
&=\mathbb{E}_W\mathbb{E}\big(Y\ |\ t,W\big)\\
\end{aligned}
$$
So that:
$$
\begin{aligned}
\mathbb{E}\big[Y\ |\ \text{do}(T=1)\big]-\mathbb{E}\big[Y\ |\ \text{do}(T=0)\big]&=\mathbb{E}_W\mathbb{E}\big(Y\ |\ T=1,W\big)-\mathbb{E}_W\mathbb{E}\big(Y\ |\ T=0,W\big)\\
&=\mathbb{E}_W\Big[\mathbb{E}\big[Y|T=1,W\big]-\mathbb{E}\big[Y|T=0,W\big]\Big]\\
&=\mathbb{E}\big[Y(1)-Y(0)\big]\\
&=\tau\quad\quad\quad\quad\quad\quad\quad\quad\text{(ATE in Chapter 2)}
\end{aligned}
$$
*This indicates that we should simply choose $W$ so that the backdoor criterion is satisfied.*

## 4.4 Structural Causal Models (SCMs)

### Definitions

**Unobserved Random Variable:**
$$
U
$$
**Structural Equation:**
$$
B:=f(A)
$$
**Structural Equation with Noise:**
$$
B:=f(A,U)
$$
<img src="figs\4.7.png" style="zoom:55%;" />

**Cause:** $X$ is the cause of $Y$ if $Y$ is reachable to $X$.

**Direct Cause:** $X$ is the direct cause of $Y$ if $Y$ is directly reachable to $X$.

**Endogenous Variables:** Variables who do have parent(s) in the causal graph.

**Exogenous Variables:** Variables who <u>do not</u> have any parents in the causal graph.

### Structural Causal Model (SCM)

A structural causal model is a tuple of the following sets:

1. A set of endogenous variables $V$.
2. A set of exogenous variables $U$.
3. A set of functions $f$, one to generate each endogenous variable as a function of other variables.

|        Type        |                     Structural Equation                      |                 Causal Graph                  |
| :----------------: | :----------------------------------------------------------: | :-------------------------------------------: |
|        SCM         | $M:\quad\begin{aligned}B&:=f_B(A,U_B)\\C&:=f_C(A,B,U_C)\\D&:=f_D(A,C,U_D)\end{aligned}$ | <img src="figs\4.8.png" style="zoom:50%;" />  |
|        SCM         | $M:\quad\begin{aligned}T&:=f_T(X,U_T)\\Y&:=f_Y(X,T,U_Y)\end{aligned}$ | <img src="figs\4.9.png" style="zoom:50%;" />  |
| Interventional SCM | $M_t:\quad\begin{aligned}T&:=t\\Y&:=f_Y(X,T,U_Y)\end{aligned}$ | <img src="figs\4.10.png" style="zoom:50%;" /> |

### The Law of Counterfactuals

$$
Y_i(t)=Y_i(M_t)
$$

Given an SCM with enough details about it specified, we can actually compute counterfactuals.

## 4.5 Example

Check the textbook for details.





# 5 Randomized Experiments

> ***Method to construct exchangeability.***

## 5.1 What is Randomized Experiments

**Randomized Experiments:** Reconstruct $T$ randomly to get $T'$ and discuss the new association $T'\Longrightarrow Y$.

This method requires the complete control over the treatment assignment mechanism.

In randomized experiments, association $T'\Longrightarrow Y$ is causation.

## 5.2 Why *Association is Causation* in Randomized Experiments

### Perspective 1: Covariate Balance

**Covariate Balance:** We have covariate balance if the distribution of covariates $X$ is the same across treatment groups.
$$
P\big(X\ |\ T'=0\big)\overset{d}{=}P\big(X\ |\ T'=1\big)
$$
<img src="figs\5.a.png" style="zoom:60%;" />

With $T$ randomly shuffled, the cause $X$ for any $T'=t'$ remains the same, which indicates the covariate balance:
$$
\begin{aligned}
&\begin{cases}
P\big(X\ |\ T'=0\big)\overset{d}{=}P\big(X\big)\\
P\big(X\ |\ T'=1\big)\overset{d}{=}P\big(X\big)
\end{cases}\\
\Longrightarrow&\quad
P\big(X\ |\ T'=0\big)\overset{d}{=}P\big(X\ |\ T'=1\big)
\end{aligned}
$$
In other words, $X$ is independent from $T'$.

Proof of *association is causation:*
$$
\begin{aligned}
P\big(y\ |\ do(t)\big)&=\sum_xP(y\ |\ t,x)P(x)\quad\text{(Backdoor Adjustment)}\\
&=\sum_xP(y\ |\ t,x)P(x\ |\ t)\quad\text{(Independence)}\\
&=\sum_xP(y,x\ |\ t)\\
&=P(y\ |\ t)\\
\end{aligned}
$$

### Perspective 2: Exchangeability

As the two groups $T'=0,\ T'=1$ are all randomly selected, we get the exchangeability:
$$
\begin{aligned}
&\mathbb{E}\big[Y(0)|T'=0\big]=\mathbb{E}\big[Y(0)|T'=1\big]\\
&\mathbb{E}\big[Y(1)|T'=0\big]=\mathbb{E}\big[Y(1)|T'=1\big]
\end{aligned}
$$
With the consistency assumption, we can easily prove that: <!--section 2.3-->
$$
\tau=\mathbb{E}\big[Y|T'=1\big]-\mathbb{E}\big[Y|T'=0\big]
$$

### Perspective 3: No Backdoor Paths

<img src="figs\5.b.png" style="zoom:60%;" />

Similar to covariate balance, we can using backdoor adjustment to get a direct proof:
$$
P\big(y\ |\ do(t)\big)=P\big(y\ |\ t\big)
$$
where the sufficient adjustment set for $T'\Longrightarrow Y$ is an empty set.





# 6 Nonparametric Identification

> ***Necessary and sufficient conditions for multiple variable interventions.***

## 6.1 Frontdoor Adjustment

The frontdoor adjustment can get identifiability without blocking all backdoor paths.

### Example Steps for Frontdoor Adjustment

<img src="figs\6.3.png" style="zoom:55%;" />

#### Step 1

There is no backdoor path as $Y$ is a collider on the path $T\leftarrow W\rightarrow Y\leftarrow M$.

Using the backdoor adjustment conditioned on an empty set we get:
$$
P\big(m\ |\ \text{do}(t)\big)=P\big(m\ |\ t\big)
$$

#### Step 2

There exists a backdoor path $M\leftarrow T\leftarrow W\rightarrow Y$.

Using the backdoor adjustment conditioned on $T$ we get:
$$
P\big(y\ |\ \text{do}(t)\big)=\sum_{t'}P\big(y\ |\ m,t'\big)P\big(t'\big)
$$

#### Step 3

To deduce $P\big(y\ |\ \text{do}(t)\big)$, we need to combine step 1&2 together:
$$
\begin{aligned}
P\big(y\ |\ \text{do}(t)\big)&=\sum_mP\big(y\ |\ \text{do}(t),m\big)\\
&=\sum_mP\big(m\ |\ \text{do}(t)\big)P\big(y\ |\ m\big)\\
&=\sum_mP\big(m\ |\ \text{do}(t)\big)P\big(y\ |\ \text{do}(m)\big)\quad\text{(M is the causation of Y)}\\
&=\sum_mP\big(m\ |\ t\big)\sum_{t'}P\big(y\ |\ m,t'\big)P\big(t'\big)\quad\text{(Step 1, Step 2)}\\
\end{aligned}
$$

### Frontdoor Criterion

A set of variables $M$ satisfies the frontdoor criterion relative to $T$ and $Y$ if the following are true:

1. $M$ completely mediates the effect of $T$ on $Y$.

   i.e., all causal paths from $T$ to $Y$ go through $M$.

2. There is no backdoor path from $T$ to $M$. **(Step 1)**

3. All backdoor paths from $M$ to $Y$ are blocked by $T$. **(Step 2)**

### Conclusion

If $(T, M, Y)$ satisfy the frontdoor criterion and we have positivity, then:
$$
P\big(y\ |\ \text{do}(t)\big)=\sum_mP\big(m\ |\ t\big)\sum_{t'}P\big(y\ |\ m,t'\big)P\big(t'\big)
$$
Proof: Check the textbook for details.

## 6.2 do-calculus

















## 6.3 Determining Identifiability from the Graph














