# Introduction to Causal Inference

This is a brief note on [Brady Neal](https://www.bradyneal.com/aboutme)'s online causal inference course. The Content is mainly arranged by the course textbook. Some sections are slightly modified according to personal comprehension to help understanding. *Last update on August 24th, 2022.*

This course covers both SCM and RCM in causal inference:

1. SCM: Mainly about Structural Causal Model (SCM) framework.
2. RCM: Mainly about Rubin Causal Model (RCM), a.k.a, Potential Outcome framework (PO).

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

> ***Distinguish causation from association.***

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
&=\mathbb{E}_X\Big[\mathbb{E}\big[Y(1)|T=1,X\big]-\mathbb{E}\big[Y(0)|T=0,X\big]\Big]\quad\text{(Unconfoundedness \& Positivity)}\\
&=\mathbb{E}_X\Big[\mathbb{E}\big[Y|T=1,X\big]-\mathbb{E}\big[Y|T=0,X\big]\Big]\quad\text{(Consistency)}
\end{aligned}
$$

### Stable Unit-treatment Value Assumption (SUTVA)

A combination of consistency and no interference.

## 2.4 Fancy Statistics Terminology De-fancified

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

- Given: $P$ is <u>Markov distribution</u> with respect to $G$.

  If $X,Y$ are d-separated by $Z$ in graph $G$, then $X,Y$ are independent in the distribution $P$ conditioned on $Z$.
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

where $\text{pa}_i$ denotes the parents of $x_i$.

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
In other words, $X$ is independent of $T'$.

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

> ***Necessary and sufficient conditions for indentifiability.***

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

### Fundamental Concepts

$G_{\overline{X}}$: Graph with all incoming edges to nodes in set $X$ removed.

$G_{\underline{X}}$: Graph with all outgoing edges to nodes in set $X$ removed.

$⫫_G$: Independent in graph $G$.

### Rules of do-calculus

Given a causal graph $G$, an associated distribution $P$, and disjoint sets of variables $Y,T,Z,W$, the following rules hold:

#### Rule 1 (remove $Z$)

$$
P\big(y\ |\ \text{do}(t),z,w\big)=P\big(y\ |\ \text{do}(t),w\big)\quad \text{if}\quad Y⫫_{G_\overline{T}}Z\ |\ T,W
$$

#### Rule 2 (convert $Z\leftrightarrow\text{do}(z)$)

$$
P\big(y\ |\ \text{do}(t),\text{do}(z),w\big)=P\big(y\ |\ \text{do}(t),z,w\big)\quad \text{if}\quad Y⫫_{G_{\overline{T},\underline{Z}}}Z\ |\ T,W
$$

#### Rule 3 (remove $\text{do}(z)$)

$$
P\big(y\ |\ \text{do}(t),\text{do}(z),w\big)=P\big(y\ |\ \text{do}(t),w\big)\quad \text{if}\quad Y⫫_{G_{\overline{T},\overline{Z(W)}}}Z\ |\ T,W
$$

where $Z(W)$ denotes the set of nodes of $Z$ that aren’t ancestors of any node of $W$ in $G_\overline{T}$.

**Complete Proof with Graph Theory:** [(1994) Causal diagrams for empirical research.pdf](materials\(1994) Causal diagrams for empirical research.pdf) 

**Proof of Completeness:**

-  [(2006-AAAI) Identification of Joint Interventional Distributions in Recursive Semi-Markovian Causal Models.pdf](materials\proofs of completeness on do-calculus\(2006-AAAI) Identification of Joint Interventional Distributions in Recursive Semi-Markovian Causal Models.pdf) 
-  [(2012) Pearl's Calculus of Intervention Is Complete.pdf](materials\proofs of completeness on do-calculus\(2012) Pearl's Calculus of Intervention Is Complete.pdf) 
-  [(2012) Identification of Conditional Interventional Distributions.pdf](materials\proofs of completeness on do-calculus\(2012) Identification of Conditional Interventional Distributions.pdf) 

## 6.3 Determining Identifiability from the Graph

The backdoor and frontdoor criteria have given identifiability under certain circumstances. However, there still exists plenty of causal estimands that don’t satisfy these two criteria. Those more general criteria are discussed as follows.

### Single Variable Intervention

**Unconfounded Children Criterion:** Given a treatment set $T$ and a single observed outcome variable $Y$, we define $M$ as a set of nodes that are the children of $T$ as well as the ancestors of $Y$. <u>If all backdoor paths from $T$ to $M$ can be blocked by intervening on $W$, then $P\big(Y=y\ |\ \text{do}(T=t)\big)$ is identifiable.</u>

<img src="figs\6.12.png" style="zoom:55%;" />

The unconfounded children criterion is a ***sufficient*** condition for identifiability.

### Multiple Variable Interventions

A ***necessary and sufficient*** condition for an observed outcome set $Y$ is provided by **the hedge criterion**.

There also exists a more general type of causal estimand called **conditional causal effects**, formulated like $P(Y\ |\ \text{do}(t),X)$.





# 7 Estimation

> ***Models for estimation.***

## 7.1 Preliminaries

### Concepts

**ITE (Individual Treatment Effect):**
$$
\tau_i=Y_i(1)-Y_i(0)
$$
**ATE (Average Treatment Effect):**
$$
\tau=\mathbb{E}\big[Y_i(1)-Y_i(0)\big]\\
$$
**CATE (Conditional Average Treatment Effect):**
$$
\tau(x)=\mathbb{E}\big[Y_i(1)-Y_i(0)\ |\ X=x\big]\\
$$
**IATEs (Individualized Average Treatment Effects):**

When $X$ contains all exogenous variables $I_i$ that may affect the potential outcomes $Y_i$ for each individual $i$, then we call *CATE* as *IATEs*. (Formulated like $\tau(x)=\mathbb{E}\big[Y_i(1)-Y_i(0)\ |\ X=x\big],\ X=\bigcup I_i\\$, where $I_i$ is the exogenous variables that affect $Y_i$)

### Symbols

**Conditional Outcome:**
$$
\begin{aligned}
\mu(t,w)&=\mathbb{E}\big[Y\ |\ T=t,\ W=w\big]\\
\mu(t,w,x)&=\mathbb{E}\big[Y\ |\ T=t,\ W=w,\ X=x\big]\\
\end{aligned}
$$

We can rewrite ATE and CATE as follows with the new symbol:
$$
\begin{aligned}
\tau&=\mathbb{E}\big[\mu(1,w)-\mu(0,w)\big]\\
\tau(x)&=\mathbb{E}\big[\mu(1,w,x)-\mu(0,w,x)\big]
\end{aligned}
$$

### Unconfoundedness Assumption

When estimating an ATE, we assume that $W$ is a sufficient adjustment set.

When estimating a CATE, we assume that $W\cup X$ is a sufficient adjustment set.

## 7.2 Conditional Outcome Modeling (COM)

The conditional outcome model (COM) directly fits $\mu$ using a single estimator $\hat{\mu}$.

<img src="figs\7.2a.png" style="zoom:70%;" />

### Estimates

| Estimates              | Results                                                      |
| ---------------------- | ------------------------------------------------------------ |
| ITE for individual $i$ | $\hat{\tau}_i=\hat{\mu}(1,w_i)-\hat{\mu}(0,w_i)$             |
| ATE                    | $\hat{\tau}=\dfrac{1}{n}\sum_i^n\big[\hat{\mu}(1,w_i)-\hat{\mu}(0,w_i)\big]\\$ |

### Conditional Estimates

| Conditional Estimates   | Results                                                      |
| ----------------------- | ------------------------------------------------------------ |
| IATE for individual $i$ | $\hat{\tau}(x_i)=\hat{\mu}(1,w_i,x_i)-\hat{\mu}(0,w_i,x_i)$  |
| CATE                    | $\hat{\tau}(x)=\dfrac{1}{n_x}\sum_{i:x_i=x}\big[\hat{\mu}(1,w_i,x_i)-\hat{\mu}(0,w_i,x_i)\big]\\$,<br />where $n_x$ denotes the number of data points that $x_i=x$. |

Under conditioned circumstances, though IATE is different from ITE, it is common to represent ITE with IATE:
$$
\hat{\tau}_i=\hat{\tau}(x_i)=\hat{\mu}(1,w_i,x_i)-\hat{\mu}(0,w_i,x_i)
$$
Though, this will likely be unreliable due to <u>severe positivity violation</u>.

## 7.3 Grouped Conditional Outcome Modeling (GCOM)

The grouped conditional outcome model (GCOM) fits $\mu$ using two estimators $\hat{\mu}_1,\hat{\mu}_0$.

Usually, $T$ is one-dimensional and $W$ is high-dimensional, while both of them hold equal importance. It is hard for a single model to distinguish one-dimensional $T$ from the high-dimensional $T+W$ so that the importance of $T$ is reduced. To solve this problem, a heuristic method is to separate the model into two parts by the value of $T$.

<img src="figs\7.2b.png" style="zoom:70%;" />

### Estimates

| Estimates              | Results                                                      |
| ---------------------- | ------------------------------------------------------------ |
| ITE for individual $i$ | $\hat{\tau}_i=\hat{\mu}_1(w_i)-\hat{\mu}_0(w_i)$             |
| ATE                    | $\hat{\tau}=\dfrac{1}{n}\sum_i^n\big[\hat{\mu}_1(w_i)-\hat{\mu}_0(w_i)\big]\\$ |

### Conditional Estimates

| Conditional Estimates   | Results                                                      |
| ----------------------- | ------------------------------------------------------------ |
| IATE for individual $i$ | $\hat{\tau}(x_i)=\hat{\mu}_1(w_i,x_i)-\hat{\mu}_0(w_i,x_i)$  |
| CATE                    | $\hat{\tau}(x)=\dfrac{1}{n_x}\sum_{i:x_i=x}\big[\hat{\mu}_1(w_i,x_i)-\hat{\mu}_0(w_i,x_i)\big]\\$,<br />where $n_x$ denotes the number of data points that $x_i=x$. |

## 7.4 Increasing Data Efficiency

The GCOM solves the problem of unbalanced feature sizes, but it is inefficient as each model only takes in a subset of the whole dataset. There are a few structures that aim to solve this problem.

### TARNet

TARNet is structured like the Mixture of Experts (MoE) model. All treatments share a common bottom in the first few layers, while the network branches off for each treatment after the bottom layer.

<img src="figs\7.2c.png" style="zoom:70%;" />

### X-Learner

Instead of modifying the structure of the model, X-Learner modifies the calculation steps of ITE / IATE on GCOM.

Take IATE $\hat{\tau}(x_i)$ for example:

#### Step 1

Same as the standard GCOM, calculate $\hat{\mu}_1(w_i,x_i)$ and $\hat{\mu}_0(w_i,x_i)$.

#### Step 2

Specify the IATE for each treatment, calculate as follows:
$$
\hat{\tau}_1(x_i)=Y_i(1)-\hat{\mu}_0(w_i,x_i)\\
\hat{\tau}_0(x_i)=\hat{\mu}_1(w_i,x_i)-Y_i(0)
$$
With this operation, we separately use the data from two treatments. This is also where "X" comes in its name.

#### Step 3

Aggregate the specified IATE together with a weighting function $g(x)$:
$$
\hat{\tau}(x_i)=g(x)\hat{\tau}_0(x_i)+(1-g(x))\hat{\tau}_1(x_i)
$$
With this operation, we aggregate the data from two treatments and estimate IATE from the whole dataset.

## 7.5 Propensity Scores

Use a model to squeeze $W$ into a one-dimensional propensity score $e(W)$ and treat it as the new condition.
$$
W\quad\Longrightarrow\quad  e(W)\\
\big(Y(1)-Y(0)\big)⫫T\ |\ W\quad\Longrightarrow\quad\big(Y(1)-Y(0)\big)⫫T\ |\ e(W)
$$
<img src="figs\7.4.png" style="zoom:55%;" />

### Inverse Probability Weighting (IPW)

We can also make model-free prediction by reweighting data so that $T⫫W$ when $e(W)=P(Y=1|W)$.

In other words, remove the association between $T$ and $W$, following the same principle with randomized experiments.
$$
\begin{aligned}
\tau&=\mathbb{E}_W\Big[\mathbb{E}\big[Y|T=1,W\big]-\mathbb{E}\big[Y|T=0,W\big]\Big]\\
&=\mathbb{E}_W\Big[\mathbb{E}\big[Y|T=1,W\big]\Big]-\mathbb{E}_W\Big[\mathbb{E}\big[Y|T=0,W\big]\Big]\quad\text{(T is independent of W)}\\
&=\mathbb{E}\bigg[\dfrac{\mathbb{1}(T=1)Y}{P(T=1|W)}\bigg]-\mathbb{E}\bigg[\dfrac{\mathbb{1}(T=0)Y}{P(T=0|W)}\bigg]\quad\text{(Appendix A.3 in course book)}\\
&=\mathbb{E}\bigg[\dfrac{\mathbb{1}(T=1)Y}{e(W)}\bigg]-\mathbb{E}\bigg[\dfrac{\mathbb{1}(T=0)Y}{1-e(W)}\bigg]
\end{aligned}
$$
where $\mathbb{1}(T=t)Y=\begin{cases}Y,\quad T=t\\0,\quad\ T\ne t\end{cases}$.

### Doubly Robust Methods

Combine $\mu(t,w)$ and $e(W)$ together.

We can construct a model $\hat{\mu}$ following the above methods on $T,e(W)$ instead of $T,W$ to predict $\tau$.

## 7.6 Other Methods

Matching, Double Machine Learning, Causal Trees and Forests, etc.

## 7.7 Concluding Remarks

Calculate confidence intervals on these estimates is necessary.

<u>**Comparison to Randomized Experiments:** These methods only address observed confounding, while randomized experiments also eliminates unobserved confounding.</u>





# 8 Unobserved Confounding: Bounds and Sensitivity Analysis

> ***Trade-off between precision and assumptions.***

<u>***Note:** Be sure to refer to the proofs and examples on the course book to help understanding.*</u>

## 8.1 Bounds

**The Law of Decreasing Credibility:** The credibility of inference decreases with the strength of the assumptions maintained.

This section considers some weaker assumptions which give the intervals where $\tau$ will fall rather than giving a specific score with the assumption of unconfoundedness.

We take the medical treatment as an example. The treatment $T=1$ denotes taking medication while $T=0$ denotes not taking it. And $Y$ denotes the outcome that whether the patient survived or not.

We care about the sign of $\tau=\mathbb{E}\big[Y(1)-Y(0)\big]$ that denotes whether potential outcome of taking medication $Y(1)$ is better than not taking it $Y(0)$.

### Plain Bound

To begin with, we need to assume a basic bound for the potential outcomes.

**Bounded Potential Outcomes:**
$$
a\le Y(t)\le b,\quad\forall t
$$
We can directly get the bound for $\mathbb{E}\big[Y(1)-Y(0)\big]$ from the bounded potential outcomes:<!--Textbook P74-->
$$
a-b\le\mathbb{E}\big[Y(1)-Y(0)\big]\le b-a
$$

### No-Assumptions Bound

The plain bound can be narrowed with no extra assumptions introduced via decomposition.

**Observational-Counterfactual Decomposition:**
$$
\begin{aligned}
\mathbb{E}\big[Y(1)-Y(0)\big]=&\quad\ \pi\mathbb{E}\big[Y(1)\ |\ T=1\big]+(1-\pi)\mathbb{E}\big[Y(1)\ |\ T=0\big]\\
&-\pi\mathbb{E}\big[Y(0)\ |\ T=1\big]-(1-\pi)\mathbb{E}\big[Y(0)\ |\ T=0\big]\\
\\
=&\quad\ \pi\mathbb{E}\big[Y\ |\ T=1\big]+(1-\pi)\mathbb{E}\big[Y(1)\ |\ T=0\big]\\
&-\pi\mathbb{E}\big[Y(0)\ |\ T=1\big]-(1-\pi)\mathbb{E}\big[Y\ |\ T=0\big]\\
\end{aligned}
$$
where $\pi\overset{\Delta}{=}P(T=1)$ for short.

- We can get $\mathbb{E}\big[Y\ |\ T=1\big],\ \mathbb{E}\big[Y\ |\ T=0\big]$ directly from observation.
- We can't get $\mathbb{E}\big[Y(0)\ |\ T=1\big],\ \mathbb{E}\big[Y(1)\ |\ T=0\big]$ as they are counterfactuals.

We can get a tighter bound with observational-counterfactual decomposition applied:<!--Textbook P75-->

$$
\mathbb{E}\big[Y(1)-Y(0)\big]\le\pi\mathbb{E}\big[Y\ |\ T=1\big]+(1-\pi)b-\pi a-(1-\pi)\mathbb{E}\big[Y\ |\ T=0\big]\\
\mathbb{E}\big[Y(1)-Y(0)\big]\ge\pi\mathbb{E}\big[Y\ |\ T=1\big]+(1-\pi)a-\pi b-(1-\pi)\mathbb{E}\big[Y\ |\ T=0\big]
$$

### Monotone Treatment Response (MTR)

#### Nonnegative MTR

This assumes that the treatment can only help (e.g., taking elixir):
$$
Y_i(1)\ge Y_i(0),\ \forall i
$$
This is equal to:
$$
\mathbb{E}\big[Y(1)\ |\ T=1\big]\ge\mathbb{E}\big[Y(0)\ |\ T=1\big]\\
\mathbb{E}\big[Y(1)\ |\ T=0\big]\ge\mathbb{E}\big[Y(0)\ |\ T=0\big]
$$
We can get the <u>lower bound</u> for nonnegative MTR:<!--Textbook P77-->
$$
\mathbb{E}\big[Y(1)-Y(0)\big]\ge0
$$

#### Nonpositive MTR

This assumes that the treatment can only hurt (e.g., taking poison):
$$
Y_i(1)\le Y_i(0),\ \forall i
$$
This is equal to:
$$
\mathbb{E}\big[Y(1)\ |\ T=1\big]\le\mathbb{E}\big[Y(0)\ |\ T=1\big]\\
\mathbb{E}\big[Y(1)\ |\ T=0\big]\le\mathbb{E}\big[Y(0)\ |\ T=0\big]
$$
We can get the <u>upper bound</u> for nonpositive MTR:<!--Textbook P77-->
$$
\mathbb{E}\big[Y(1)-Y(0)\big]\le0
$$

### Monotone Treatment Selection (MTS)

**(Nonnegative MTS)** This assumes that treatment groups’ potential outcomes are better than control groups’:
$$
\mathbb{E}\big[Y(1)\ |\ T=1\big]\ge\mathbb{E}\big[Y(1)\ |\ T=0\big]\\
\mathbb{E}\big[Y(0)\ |\ T=1\big]\ge\mathbb{E}\big[Y(0)\ |\ T=0\big]
$$
<u>*MTS focuses on the group, while MTR focuses on the outcome.*</u>

We can get the <u>upper bound</u> for (Nonnegative) MTS:<!--Textbook P78-->
$$
\mathbb{E}\big[Y(1)-Y(0)\big]\le\mathbb{E}\big[Y\ |\ T=1\big]-\mathbb{E}\big[Y\ |\ T=0\big]
$$

### Optimal Treatment Selection (OTS)

This assumes that the individuals always receive the treatment that is best for them:
$$
T_i=0\quad\Longleftrightarrow\quad Y_i(0)\ge Y_i(1)\\
T_i=1\quad\Longleftrightarrow\quad Y_i(0)< Y_i(1)
$$

#### OTS Bound 1

From OTS, we can deduce that:
$$
\mathbb{E}\big[Y(1)\ |\ T=1\big]\ge\mathbb{E}\big[Y(0)\ |\ T=1\big]\\
\mathbb{E}\big[Y(0)\ |\ T=0\big]\ge\mathbb{E}\big[Y(1)\ |\ T=0\big]
$$
So we can get a bound with the above condition applied:<!--Textbook P79-->
$$
\begin{aligned}
\mathbb{E}\big[Y(1)-Y(0)\big]&\le\pi\mathbb{E}\big[Y\ |\ T=1\big]-\pi a\\
\mathbb{E}\big[Y(1)-Y(0)\big]&\ge(1-\pi)a-(1-\pi)\mathbb{E}\big[Y\ |\ T=0\big]
\end{aligned}
$$

#### OTS Bound 2

From OTS, we can also deduce that:
$$
\mathbb{E}\big[Y(1)\ |\ T=1\big]\ge\mathbb{E}\big[Y(1)\ |\ T=0\big]\\
\mathbb{E}\big[Y(0)\ |\ T=0\big]\ge\mathbb{E}\big[Y(0)\ |\ T=1\big]
$$
So we can get a bound with the above condition applied:<!--Textbook P81-->
$$
\begin{aligned}
\mathbb{E}\big[Y(1)-Y(0)\big]&\le\mathbb{E}\big[Y\ |\ T=1\big]-\pi a-(1-\pi)\mathbb{E}\big[Y\ |\ T=0\big]\\
\mathbb{E}\big[Y(1)-Y(0)\big]&\ge\pi\mathbb{E}\big[Y\ |\ T=1\big]+(1-\pi)a-\mathbb{E}\big[Y\ |\ T=0\big]
\end{aligned}
$$

#### Mixing Bounds

Combine the two OTS bounds together, we can get a tighter bound:
$$
\begin{aligned}
\text{if}\ \ \mathbb{E}\big[Y\ |\ T=0\big]\le\mathbb{E}\big[Y\ |\ T=1\big]&:\\
\mathbb{E}\big[Y(1)-Y(0)\big]&\le\pi\mathbb{E}\big[Y\ |\ T=1\big]-\pi a\\
\mathbb{E}\big[Y(1)-Y(0)\big]&\ge\pi\mathbb{E}\big[Y\ |\ T=1\big]+(1-\pi)a-\mathbb{E}\big[Y\ |\ T=0\big]\\
\\
\text{if}\ \ \mathbb{E}\big[Y\ |\ T=0\big]>\mathbb{E}\big[Y\ |\ T=1\big]&:\\
\mathbb{E}\big[Y(1)-Y(0)\big]&\le\mathbb{E}\big[Y\ |\ T=1\big]-\pi a-(1-\pi)\mathbb{E}\big[Y\ |\ T=0\big]\\
\mathbb{E}\big[Y(1)-Y(0)\big]&\ge(1-\pi)a-(1-\pi)\mathbb{E}\big[Y\ |\ T=0\big]
\end{aligned}
$$

## 8.2 Sensitivity Analysis

This section discusses the effect of unobserved confounders on the calculated results.

### Linear Setting

<img src="figs\8.3.png" style="zoom:55%;" />
$$
\begin{aligned}
T&:=\alpha_wW+\alpha_uU\\
Y&:=\beta_wW+\beta_uU+\delta T\\
\end{aligned}
$$

#### Confounder Bias

The ATE we get when conditioning on $W,U$:<!--Textbook P83-->
$$
\begin{aligned}
\tau_{w,u}&=\mathbb{E}\big[Y(1)-Y(0)\big]\\
&=\mathbb{E}_{W,U}\Big[\mathbb{E}\big[Y\ |\ T=1,W,U\big]-\mathbb{E}\big[Y\ |\ T=0,W,U\big]\Big]\\
&=\delta
\end{aligned}
$$
The ATE we get when conditioning on $W$:<!--Textbook P83-->
$$
\begin{aligned}
\tau_{w}&=\mathbb{E}\big[Y(1)-Y(0)\big]\\
&=\mathbb{E}_{W}\Big[\mathbb{E}\big[Y\ |\ T=1,W\big]-\mathbb{E}\big[Y\ |\ T=0,W\big]\Big]\\
&=\delta+\dfrac{\beta_u}{\alpha_u}
\end{aligned}
$$
So we get the bias from the unobserved confounder $U$:
$$
\begin{aligned}
\text{bias}&=\tau_{w,u}-\tau_{w}\\
&=\delta+\dfrac{\beta_u}{\alpha_u}-\delta\\
&=\dfrac{\beta_u}{\alpha_u}
\end{aligned}
$$

#### Sensitivity Contour Plots

To explicitly show the effect of bias on the outcome, we can check the contour plots.

Left: Contour of bias $\dfrac{\beta_u}{\alpha_u}$.

Right: Contour of $\delta$ when $\tau_{w}=\delta+\dfrac{\beta_u}{\alpha_u}=25$.

<img src="figs\8.5.png" style="zoom:65%;" />

### More General Settings

**Extend $T$ to nonlinear form:**

[(2003) Sensitivity to Exogeneity Assumptions in Program Evaluation.pdf](materials\sensitivity analysis\(2003) Sensitivity to Exogeneity Assumptions in Program Evaluation.pdf) 

**Extend to nonparametric form:**

[(2020) Making Sense of Sensitivity Extending Omitted Variable Bias.pdf](materials\sensitivity analysis\(2020) Making Sense of Sensitivity Extending Omitted Variable Bias.pdf) 

**Many other options:**

Check the textbook.





# 9 Instrumental Variables

> ***Estimate with unobserved confounders.***

## 9.1 Preliminaries

<!--It seems that this is a stronger assumption based on the Unconfounded Children Criterion.-->

**Instrument:**

A variable $Z$ can be considered as an instrument if the following assumptions are satisfied:

1. Relevance: $Z$ has a causal effect on $T$.
2. Exclusion Restriction: The causal effect of $Z$ on $Y$ is fully mediated by $T$.
3. Instrumental Unconfoundedness: There are no backdoor paths from $Z$ to $Y$.

**Conditional Instrument:**

1. Relevance.
2. Exclusion Restriction.
3. **Conditional** Instrumental Unconfoundedness: There are no backdoor paths from $Z$ to $Y$ <u>conditioned on $W$</u>.

## 9.2 Parametric Situations

The instrument variables allow us to find the causal effect of $T$ on $Y$, but under specified conditions.

<u>Specifically, the causal model must have a parametric form, e.g. linear.</u>

<img src="figs\9.1.png" style="zoom:60%;" />

We assume that the outcome $Y$ is in a linear form:
$$
Y:=\delta T+\alpha_uU
$$

### Binary Linear Setting

In this setting we have $T,Z\in\{0,1\}$.

By conditioning on $T$, we can get the **Wald Estimand**:
$$
\delta=\dfrac{\mathbb{E}\big[Y|Z=1\big]-\mathbb{E}\big[Y|Z=0\big]}{\mathbb{E}\big[T|Z=1\big]-\mathbb{E}\big[T|Z=0\big]}
$$
Proof:
$$
\begin{aligned}
\mathbb{E}\big[Y|Z=1\big]-\mathbb{E}\big[Y|Z=0\big]&=\mathbb{E}\big[\delta T+\alpha_uU|Z=1\big]-\mathbb{E}\big[\delta T+\alpha_uU|Z=0\big]\\
&=\delta\Big(\mathbb{E}\big[T|Z=1\big]-\mathbb{E}\big[T|Z=0\big]\Big)+\alpha_u\Big(\mathbb{E}\big[U|Z=1\big]-\mathbb{E}\big[U|Z=0\big]\Big)\\
&=\delta\Big(\mathbb{E}\big[T|Z=1\big]-\mathbb{E}\big[T|Z=0\big]\Big)+\alpha_u\Big(\mathbb{E}\big[U\big]-\mathbb{E}\big[U\big]\Big)\quad\text{(U is independent of Z)}\\
&=\delta\Big(\mathbb{E}\big[T|Z=1\big]-\mathbb{E}\big[T|Z=0\big]\Big)
\end {aligned}
$$
As each term in the Wald Estimand can be observed, we can directly get the causal effect.

### Continuous Linear Setting

In this setting $T$ and $Z$ are continuous rather than binary.

Similar to the binary setting, we can get the **Wald Estimand**:
$$
\delta=\dfrac{\text{Cov}(Y,Z)}{\text{Cov}(T,Z)}
$$
where $\text{Cov}$ denotes the covariance.

Proof:
$$
\begin{aligned}
\text{Cov}(Y,Z)&=\mathbb{E}\big[YZ\big]-\mathbb{E}\big[Y\big]\mathbb{E}\big[Z\big]\\
&=\mathbb{E}\big[(\delta T+\alpha_uU)Z\big]-\mathbb{E}\big[\delta T+\alpha_uU\big]\mathbb{E}\big[Z\big]\\
&=\delta\Big(\mathbb{E}\big[TZ\big]-\mathbb{E}\big[T\big]\mathbb{E}\big[Z\big]\Big)+\alpha_u\Big(\mathbb{E}\big[UZ\big]-\mathbb{E}\big[U\big]\mathbb{E}\big[Z\big]\Big)\\
&=\delta\Big(\mathbb{E}\big[TZ\big]-\mathbb{E}\big[T\big]\mathbb{E}\big[Z\big]\Big)+\alpha_u\Big(\mathbb{E}\big[U\big]\mathbb{E}\big[Z\big]-\mathbb{E}\big[U\big]\mathbb{E}\big[Z\big]\Big)\quad\text{(U is independent of Z)}\\
&=\delta\Big(\mathbb{E}\big[TZ\big]-\mathbb{E}\big[T\big]\mathbb{E}\big[Z\big]\Big)\\
&=\delta\ \text{Cov}(T,Z)\\
\end {aligned}
$$
So we can directly model $\hat{\delta}=\dfrac{\hat{\text{Cov}}(Y,Z)}{\hat{\text{Cov}}(T,Z)}$, or using **two-stage least squares estimator (2SLS)**.<!--Textbook P89-->

## 9.3 Nonparametric Situations

In this section we assume the binary setting that $T,Z\in\{0,1\}$.

### Fundamental Concepts

**New potential Notations:**
$$
\begin{aligned}
T(z)&=T(Z=z)\\
Y(t)&=Y(T=t)\\
\end{aligned}
$$
**Principal Strata:**

| Name          | Description                                                  | Equation          |
| ------------- | ------------------------------------------------------------ | ----------------- |
| Compliers     | Always take the treatment that they’re encouraged to take.   | $T(1)=1,\ T(0)=0$ |
| Defiers       | Always take the opposite treatment of that they are encouraged to take. | $T(1)=0,\ T(0)=1$ |
| Always-takers | Always take the treatment, regardless of encouragement.      | $T(1)=1,\ T(0)=1$ |
| Never-takers  | Never take the treatment, regardless of encouragement.       | $T(1)=0,\ T(0)=0$ |

<img src="figs\9.a.png" style="zoom:60%;" />

Given some observed value of $T$ and $Z$, we can’t actually identify which stratum we’re in. (**Can’t Identify Stratum**)

1. $T(0)=0$: compliers or never-takers.
2. $T(0)=1$: defiers or always-takers.
3. $T(1)=0$: defiers or never-takers.
4. $T(1)=1$: compliers or always-takers.

**Local Average Treatment Effect (LATE) / Complier Average Causal Effect (CACE):**
$$
\mathbb{E}\big[Y(1)-Y(0)\ |\ T(1)=1,\ T(0)=0\big]
$$
**Monotonicity Assumption:**
$$
T_i(1)\ge T_i(0),\quad\forall i
$$
This assumes that there are no defiers.

### LATE Nonparametric Identification

Given that $Z$ is an instrument, $Z$ and $T$ are binary variables and monotonicity holds, the following is true:
$$
\mathbb{E}\big[Y(1)-Y(0)\ |\ T(1)=1,\ T(0)=0\big]=\dfrac{\mathbb{E}\big[Y|Z=1\big]-\mathbb{E}\big[Y|Z=0\big]}{\mathbb{E}\big[T|Z=1\big]-\mathbb{E}\big[T|Z=0\big]}
$$
**Proof:**

First we apply the Law of Total Probability:
$$
\begin{aligned}
\mathbb{E}\big[Y(Z=1)-Y(Z=0)\big]=\ &\quad\ \mathbb{E}\big[Y(1)-Y(0)\ |\ T(1)=1,\ T(0)=0\big]P\big(T(1)=1,\ T(0)=0\big)\\
&+\mathbb{E}\big[Y(1)-Y(0)\ |\ T(1)=0,\ T(0)=1\big]P\big(T(1)=0,\ T(0)=1\big)\quad\text{(Violation of Monotonicity)}\\
&+\mathbb{E}\big[Y(1)-Y(0)\ |\ T(1)=1,\ T(0)=1\big]P\big(T(1)=1,\ T(0)=1\big)\quad\text{(No causal effects)}\\
&+\mathbb{E}\big[Y(1)-Y(0)\ |\ T(1)=0,\ T(0)=0\big]P\big(T(1)=0,\ T(0)=0\big)\quad\text{(No causal effects)}\\
=\ &\quad\ \mathbb{E}\big[Y(1)-Y(0)\ |\ T(1)=1,\ T(0)=0\big]P\big(T(1)=1,\ T(0)=0\big)\\
\end{aligned}\\
$$
We also have:
$$
\begin{aligned}
\mathbb{E}\big[Y(Z=1)-Y(Z=0)\big]&=\mathbb{E}\big[Y|Z=1\big]-\mathbb{E}\big[Y|Z=0\big]\qquad\textbf{(Instrumental Unconfoundedness)}\\
P\big(T(1)=1,\ T(0)=0\big)&=1-P\big(T(1)=1,\ T(0)=1\big)-P\big(T(1)=0,\ T(0)=0\big)\qquad\textbf{(Subtract Other Strata)}\\
&=1-P\big(T(0)=1\big)-P\big(T(1)=0\big)\qquad\textbf{(No Defiers)}\\
&=1-P\big(T(0)=1\big)-\Big(1-P\big(T(1)=1\big)\Big)\\
&=P\big(T(1)=1\big)-P\big(T(0)=1\big)\\
&=P\big(T|Z=1\big)-P\big(T|Z=1\big)\\
&=\mathbb{E}\big[T|Z=1\big]-\mathbb{E}\big[T|Z=0\big]\qquad\textbf{(Binary Setting)}\\
\end{aligned}
$$
Finally we get:
$$
\begin{aligned}
\mathbb{E}\big[Y(1)-Y(0)\ |\ T(1)=1,\ T(0)=0\big]&=\dfrac{\mathbb{E}\big[Y(Z=1)-Y(Z=0)\big]}{P\big(T(1)=1,\ T(0)=0\big)}\\
&=\dfrac{\mathbb{E}\big[Y|Z=1\big]-\mathbb{E}\big[Y|Z=0\big]}{\mathbb{E}\big[T|Z=1\big]-\mathbb{E}\big[T|Z=0\big]}
\end{aligned}
$$

## 9.4 More General Situations (Semi-parametric)

The outcome is generated by a complex function of $T$ and $W$ plus some additive unobserved confounders $U$:

$$
Y:=f(T,W)+U
$$
[(2017-ICML) Deep IV A Flexible Approach for Counterfactual Prediction.pdf](materials\instrumental variables\(2017-ICML) Deep IV A Flexible Approach for Counterfactual Prediction.pdf) 

[(2021-ICLR) Learning deep features in instrumental variable regression.pdf](materials\instrumental variables\(2021-ICLR) Learning deep features in instrumental variable regression.pdf) 

We can also give up on point identification and settle for set identification (bounds):
$$
Y:=f(T,U)
$$
[(2020-NIPS) A class of algorithms for general instrumental variable models.pdf](materials\instrumental variables\(2020-NIPS) A class of algorithms for general instrumental variable models.pdf) 





# 10 Difference in Differences

> ***Potential outcomes in the stochastic process.***

## 10.1 Preliminaries

### Fundamental Concepts

**Average Treatment Effect on the Treated (ATT):**
$$
\begin{aligned}
\mathbb{E}\big[Y(1)-Y(0)\ |\ T=1\big]&=\mathbb{E}\big[Y(1)\ |\ T=1\big]-\mathbb{E}\big[Y(0)\ |\ T=1\big]\\
&=\mathbb{E}\big[Y\ |\ T=1\big]-\mathbb{E}\big[Y(0)\ |\ T=1\big]\\
&=\mathbb{E}\big[Y\ |\ T=1\big]-\mathbb{E}\big[Y(0)\ |\ T=0\big]\quad\text{(Unconfoundness for ATT)}\\
&=\mathbb{E}\big[Y\ |\ T=1\big]-\mathbb{E}\big[Y\ |\ T=0\big]\\
\end{aligned}
$$

|      | Definition                              | Unconfoundedness        |
| ---- | --------------------------------------- | ----------------------- |
| ATE  | $\mathbb{E}\big[Y(1)-Y(0)]$             | $\big(Y(0),Y(1)\big)⫫T$ |
| ATT  | $\mathbb{E}\big[Y(1)-Y(0)\ |\ T=1\big]$ | $Y(0)⫫T$                |

To help understanding, we can treat the above ATT conditioned on $T=1$ as the ATE of the treatment group, i.e., we only care about the outcome of the treatment group. Then $Y(1)$ represents <u>the observed outcome of the treatment group</u>, while $T(0)$ represents <u>the counterfactual</u> which is the potential outcome if all treatment group members went to the control group.

Then the unconfoundedness assumption for ATT can be easily explained: As we only care about the outcome of the treatment group, we don't need to observed the counterfactual of the control group, i.e. $\mathbb{E}\big[Y(1)\ |\ T=0\big]$. So the only assumption we need is $Y(0)⫫T$.

### Introducing Time

**Observed Outcome at Time $\tau$:**
$$
Y_\tau
$$
**Potential Outcome at Time $\tau$:**
$$
Y_\tau(t)
$$
**ATT at Time $\tau$:**
$$
\mathbb{E}\big[Y_\tau(1)-Y_\tau(0)\ |\ T=1\big]
$$
 We can observe all $Y_\tau(1)$ under condition $T=1$, while $Y_\tau(0)$ are counterfactuals.

## 10.2 Identification

### Assumptions with Time Introduced

#### Consistency

$$
\begin{aligned}
&T=t\ \Longrightarrow\ Y_\tau=Y_\tau(t),\quad\forall\tau\\
&\text{i.e.}\quad Y_\tau=Y_\tau(T)
\end{aligned}
$$

#### Parallel Trends

$$
\begin{aligned}
&\mathbb{E}\big[Y_1(0)-Y_0(0)\ |\ T=1\big]=\mathbb{E}\big[Y_1(0)-Y_0(0)\ |\ T=0\big]\\
&\text{i.e.}\quad \big(Y_1(0)-Y_0(0)\big)⫫T
\end{aligned}
$$

<img src="figs\10.a.png" style="zoom:60%;" />

With time introduced, the independency changes to $\big(Y_1(0)-Y_0(0)\big)⫫T$ compared with ATT's $Y(0)⫫T$.

#### No Pretreatment Effect

$$
\mathbb{E}\big[Y_0(1)\ |\ T=1\big]=\mathbb{E}\big[Y_0(0)\ |\ T=1\big]
$$

This assumes that the observation and counterfactual are the same for treatment group at start time.

### Difference-in-differences Identification

Given consistency, parallel trends, and no pretreatment effect, we have the following:

$$
\mathbb{E}\big[Y_1(1)-Y_1(0)\ |\ T=1\big]=\Big(\mathbb{E}\big[Y_1\ |\ T=1\big]-\mathbb{E}\big[Y_0\ |\ T=1\big]\Big)-\Big(\mathbb{E}\big[Y_1\ |\ T=0\big]-\mathbb{E}\big[Y_0\ |\ T=0\big]\Big)
$$
<img src="figs\10.b.png" style="zoom:60%;" />

Proof:
$$
\begin{aligned}
\mathbb{E}\big[Y_1(1)-Y_1(0)\ |\ T=1\big]&=\mathbb{E}\big[Y_1(1)\ |\ T=1\big]-\mathbb{E}\big[Y_1(0)\ |\ T=1\big]\\
&=\mathbb{E}\big[Y_1\ |\ T=1\big]-\mathbb{E}\big[Y_1(0)\ |\ T=1\big]\quad\text{(Consistency)}\\
&=\mathbb{E}\big[Y_1\ |\ T=1\big]-\Big(\mathbb{E}\big[Y_0(0)\ |\ T=1\big]+\mathbb{E}\big[Y_1(0)\ |\ T=0\big]-\mathbb{E}\big[Y_0(0)\ |\ T=0\big]\Big)\quad\text{(Parallel Trends)}\\
&=\mathbb{E}\big[Y_1\ |\ T=1\big]-\mathbb{E}\big[Y_0(0)\ |\ T=1\big]-\mathbb{E}\big[Y_1\ |\ T=0\big]+\mathbb{E}\big[Y_0\ |\ T=0\big]\\
&=\mathbb{E}\big[Y_1\ |\ T=1\big]-\mathbb{E}\big[Y_0(1)\ |\ T=1\big]-\mathbb{E}\big[Y_1\ |\ T=0\big]+\mathbb{E}\big[Y_0\ |\ T=0\big]\quad\text{(No Pretreatment Effect)}\\
&=\Big(\mathbb{E}\big[Y_1\ |\ T=1\big]-\mathbb{E}\big[Y_0\ |\ T=1\big]\Big)-\Big(\mathbb{E}\big[Y_1\ |\ T=0\big]-\mathbb{E}\big[Y_0\ |\ T=0\big]\Big)
\end{aligned}
$$

## 10.3 Major Problems

The problem focuses on the parallel trends assumption.

### Violations of Time

Sometimes, we need to condition on $W$ to satisfy the parallel trends assumption:
$$
\begin{aligned}
&\mathbb{E}\big[Y_1(0)-Y_0(0)\ |\ T=1,W\big]=\mathbb{E}\big[Y_1(0)-Y_0(0)\ |\ T=0,W\big]\\
&\text{i.e.}\quad \big(Y_1(0)-Y_0(0)\big)⫫T,W
\end{aligned}
$$
However, if $Y$ is related to time $\tau$ and treatment $T$ together in a single term, then it is invalid by conditioning on $W$:
$$
Y:=\cdots+\tau T\quad\Longrightarrow\quad\text{Parallel Trends Violation}
$$

### Scale-Specific Problem

The parallel trends assumptions isn’t nonparametric, as it doesn't support non-linear transformation:
$$
\mathbb{E}\big[Y_1(0)-Y_0(0)\ |\ T=1\big]=\mathbb{E}\big[Y_1(0)-Y_0(0)\ |\ T=0\big]\\
\text{Does not imply}\\
\mathbb{E}\big[\log Y_1(0)-\log Y_0(0)\ |\ T=1\big]=\mathbb{E}\big[\log Y_1(0)-\log Y_0(0)\ |\ T=0\big]
$$





# 11 Causal Discovery from Observational Data

> ***Construct causality from observations.***

## 11.1 Independence-Based Causal Discovery

### Preliminaries

**Markov Assumption:** <!--copy from chapter 3-->

- If $X,Y$ are d-separated by $Z$ in graph $G$, then $X,Y$ are independent in the distribution $P$ conditioned on $Z$.

$$
X⫫_GY\ |\ Z\Longrightarrow X⫫_PY\ |\ Z
$$

**Faithfulness Assumption:**

- If $X,Y$ are independent in distribution $P$ conditioned on $Z$, then $X,Y$ are d-separated by $Z$ in graph $G$.

$$
X⫫_GY\ |\ Z\Longleftarrow X⫫_PY\ |\ Z
$$

This is the converse of the Markov assumption. It is a strong assumption and is hard to satisfy.

In reality, what we can observe is usually the distribution $P$. With Faithfulness satisfied, we can reconstruct $G$ with no bias.

**Causal Sufficiency Assumption:**

- There are no unobserved confounders of any of the variables in the graph.

### Markov Equivalence

Under the Markov, faithfulness, causal sufficiency, and acyclicity assumptions, we can partially identify the causal graph.

#### Fundamental Concepts

**Markov Equivalent:** Two graphs are Markov equivalent if they correspond to the same set of conditional independencies.

<img src="figs\11.2.png" style="zoom:60%;" />

The conditional independences $X_1⫫X_3\ |\ X_2$ are all the same in the above 3 graphs. So we can't specify the structure of corresponding causal graph $G$ with given distribution $P$. 

**Skeleton:** The structure we get if we replace all of the directed edges with undirected edges for a graph.

<img src="figs\11.4.png" style="zoom:55%;" />

**Markov Equivalence Class:** The set of graphs that encode the same conditional independencies.

<img src="figs\11.3.png" style="zoom:46%;" />

Sharing the same skeleton doesn't imply the same Markov equivalence class. Compared to the three graphs above, the immorality is in its own Markov equivalence class.

#### Markov Equivalence via Immoral Skeletons

Two graphs are Markov equivalent if and only if they have the same <u>skeleton</u> and same <u>immoralities</u>.

#### Markov Completeness

If we have multinomial distributions or linear Gaussian structural equations, we can only identify a graph up to its <u>Markov equivalence class</u>.

[(1990) Equivalence and Synthesis of Causal Models.pdf](materials\causality in observational data\(1990) Equivalence and Synthesis of Causal Models.pdf) 

#### The PC Algorithm

Starting with a complete graph, the PC algorithm continually trims down edges and orients the left ones.

1. Identify the skeleton.
2. Identify immoralities and orient them.
3. Orient qualifying edges that are incident on colliders.

<img src="figs\11.a.png" style="zoom:60%;" />

## 11.2 Semi-Parametric Causal Discovery

### Preliminaries

**Non-Identifiability of Two-Node Graphs:**

- For every joint distribution $P(x,y)$ on two real-valued random variables, there is an SCM in either direction that generates data consistent with $P(x,y)$.

$$
P(x,y)\quad\Longrightarrow\quad
\begin{cases}
Y=f_Y(X,U_Y),\quad X⫫U_Y\\
X=f_X(Y,U_X),\quad Y⫫U_X
\end{cases}
$$

To distinguish the causal relationship between two nodes, we have to make some assumptions about the functional form. But it is not necessary to assume the entire function, i.e., we make <u>semi-parametric assumptions</u>.

### Linear Non-Gaussian Noise

#### Fundamental Concepts

We can identify the direction of causal flow between $X$ and $Y$ if its structural equation follows:
$$
Y:=f(X)+U,\quad X⫫U
$$
where $f$ is a linear function, and $U$ is distributed as a non-Gaussian random variable.

#### Identifiability in Linear Non-Gaussian Setting

In the linear non-Gaussian setting with $P(x,y)$ given, if the true SCM is:
$$
Y:=f(X)+U,\quad X⫫U
$$
then there doesn't exist an SCM in the reverse direction:
$$
X:=f(Y)+\tilde{U},\quad X⫫\tilde{U}
$$

### Nonlinear Models

#### Nonlinear Additive Noise Setting

We can also get the identifiability of the causal graph when:
$$
X_i:=f(\text{pa}_i)+U_i,\quad \forall i
$$
where $f$ is a non-linear function, $\text{pa}$ is the parents of $X$, and $U$ is noise.

#### Post-Nonlinear Setting

We can also add another non-linear function:
$$
X_i:=g\big(f(\text{pa}_i)+U_i\big),\quad \forall i
$$
where $f,g$ are non-linear functions, $\text{pa}$ is the parents of $X$, and $U$ is noise.

## 11.3 Further Resources

Check the following materials for the frontier of causal discovery research.

[(2017) Introduction to the foundations of causal discovery.pdf](materials\causality in observational data\(2017) Introduction to the foundations of causal discovery.pdf) 

[(2019) Review of Causal Discovery Methods Based on Graphical Models.pdf](materials\causality in observational data\(2019) Review of Causal Discovery Methods Based on Graphical Models.pdf) 





# 12 Causal Discovery from Interventional Data

> ***Construct causality from interventions.***

<u>***Note:** The content of this chapter is missing in the textbook. It's better to directly check the slide for details.*</u>

## 12.1 Structural Interventions

### Fundamental Concepts

**Structural Interventions:**
$$
\begin{aligned}
Y&:=f_\theta(A,B,C,N_Y)\\
\Longrightarrow Y&:=N'_Y
\end{aligned}
$$
<img src="figs\12.a.png" style="zoom:70%;" />

### Interventional Markov Equivalence

The Markov equivalence is the same as that in chapter 11.

#### Single-Node

**Conclusion:**

- $n – 1$ single-node interventions are sufficient and necessary to distinguish the causal effect between each pair of nodes in the worst case (complete graph), with <u>**no** empty edges</u> included.
- $n$ single-node interventions are sufficient and necessary to distinguish the causal effect between each pair of nodes in the worst case (complete graph), with <u>empty edges</u> included.

[(2006) N-1 Experiments Suffice to Determine the Causal Relations Among N Variables.pdf](materials\causality in interventional data\(2006) N-1 Experiments Suffice to Determine the Causal Relations Among N Variables.pdf) 

#### Multi-Node

**Conclusion:**

- $\lfloor \log_2n \rfloor+1$ single-node interventions are sufficient and necessary to distinguish the causal effect between each pair of nodes in the worst case (complete graph), with <u>**no** empty edges</u> included.

[(2005) On the Number of Experiments Sufficient and in the Worst Case Necessary to Identify All Causal Relations Among N Variables.pdf](materials\causality in interventional data\(2005) On the Number of Experiments Sufficient and in the Worst Case Necessary to Identify All Causal Relations Among N Variables.pdf) 

- $\lfloor \log_2c \rfloor+1$ single-node interventions are sufficient and necessary to distinguish the causal effect between each pair of nodes in the worst case (<u>non-complete graph</u>), with <u>**no** empty edges</u> included,

  where $c$ is the the size of the largest clique.

[(2008) Almost Optimal Intervention Sets for Causal Discovery.pdf](materials\causality in interventional data\(2008) Almost Optimal Intervention Sets for Causal Discovery.pdf) 

[(2014) Two Optimal Strategies for Active Learning of Causal Models from Interventional Data.pdf](materials\causality in interventional data\(2014) Two Optimal Strategies for Active Learning of Causal Models from Interventional Data.pdf) 

## 12.2 Parametric Interventions

### Fundamental Concepts

**Parametric Interventions:**
$$
\begin{aligned}
Y&:=f_\theta(A,B,C,N_Y)\\
\Longrightarrow Y&:=f_{\theta'}(A,B,C,N_Y)
\end{aligned}
$$
<img src="figs\12.b.png" style="zoom:70%;" />

### Interventional Markov Equivalence

#### Single-Node

**Theorem:**

- Two graphs augmented with single-node interventions are interventionally Markov equivalent <u>if and only if</u> they have the same skeletons and immoralities.

[(2001) Causal Discovery from Changes.pdf](materials\causality in interventional data\(2001) Causal Discovery from Changes.pdf) 

**Conclusion:**

- $n – 1$ single-node interventions are sufficient and necessary to distinguish the causal effect between each pair of nodes in the worst case (complete graph), with <u>**no** empty edges</u> included.

[(2007) Interventions and Causal Inference.pdf](materials\causality in interventional data\(2007) Interventions and Causal Inference.pdf) 

#### Multi-Node

**Theorem:**

- Given the observational data, two graphs augmented with multi-node interventions are interventionally Markov equivalent <u>if and only if</u> they have the same skeletons and immoralities.

[(2018) Characterizing and Learning Equivalence Classes of Causal DAGs under Interventions.pdf](materials\causality in interventional data\(2018) Characterizing and Learning Equivalence Classes of Causal DAGs under Interventions.pdf) 

**Conclusion:**

[(2012) Characterization and Greedy Learning of Interventional Markov Equivalence Classes of Directed Acyclic Graphs.pdf](materials\causality in interventional data\(2012) Characterization and Greedy Learning of Interventional Markov Equivalence Classes of Directed Acyclic Graphs.pdf) 

## 12.3 Miscellaneous Other Settings

Check the slide.





# 13 Transfer Learning and Transportability

> 
>

<u>***Note:** The content of this chapter is missing in the textbook. It's better to directly check the slide for details.*</u>



























# 14 Counterfactuals and Mediation

> 
>

<u>***Note:** The content of this chapter is missing in the textbook. It's better to directly check the slide for details.*</u>

























