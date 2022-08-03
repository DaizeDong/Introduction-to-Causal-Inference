# Introduction to Causal Inference

This is a brief note on [Brady Neal](https://www.bradyneal.com/aboutme)'s online causal inference course. Contents are arranged by the course textbook. Some sections are slightly modified according to my personal comprehension to help understanding. *Last update on August 1st, 2022.*

**Course Website：** [Introduction to Causal Inference (bradyneal.com)](https://www.bradyneal.com/causal-inference-course)

**Textbook：** [Introduction_to_Causal_Inference-Dec17_2020-Neal](https://www.bradyneal.com/Introduction_to_Causal_Inference-Dec17_2020-Neal.pdf)





# 1 Motivation: Why You Might Care

> ***Distinguish association and causation.***

## 1.1 Association is Not Causation

**Association:** Statistical dependence between two subjects.

**Confounding Association:** The association facilitated by a confounder.





# 2 Potential Outcomes

> ***Estimate causation with condition.***

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

### D-separation & Markov Assumption

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

**D-separation Implies Association is Causation:** Only association conducted from a chain is the causation.

<img src="figs\3.a.png" style="zoom:60%;" />

<img src="figs\3.21.png" style="zoom:70%;" />





# 4 Causal Models

> ***Estimate causation with specified conditions.***

## 4.1 Fundamental Concepts

**do-operator:** $\text{do}(t)$ / $\text{do}(T=t)$ indicates the intervention on whole samples with $T=t$.

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
This is an extended form of the regular factorization with with modularity applied.

## 4.3 The Backdoor Adjustment

### Backdoor Criterion

A set of variables $W$ satisfies the backdoor criterion relative to $T$ and $Y$ if the following are true:

1. $W$ blocks all backdoor paths from $T$ to $Y$.
2. $W$ does not contain any descendants of $T$.

**Backdoor paths:** All non-causal association paths (forks and conditioned immoralities).

#### Why to Not Condition on Descendants of Treatment

1. We block the flow of causation from $T$ to $Y$.
2. We induce non-causal association between $T$ and $Y$.

<img src="figs\4.a.png" style="zoom:55%;" />

#### Collider Bias

Unfortunately, even if we only condition on pretreatment covariates, we can still induce collider bias.

An example of **M-bias**:

<img src="figs\4.16.png" style="zoom:60%;" />

### Backdoor Adjustment

Given the modularity assumption that $W$ satisfies the backdoor criterion and positivity, we can identify the causal effect of $T$ on $Y$:
$$
P\big(y\ |\ \text{do}(t)\big)=\sum_wP\big(y\ |\ t,w\big)P\big(w\big)
$$
Proof of the backdoor adjustment:
$$
\begin{aligned}
P\big(y\ |\ \text{do}(t)\big)&=\sum_wP\big(y,w\ |\ \text{do}(t)\big)\\
&=\sum_wP\big(y\ |\ \text{do}(t),w\big)P\big(w\ |\ \text{do}(t)\big)\\
&=\sum_wP\big(y\ |\ t,w\big)P\big(w\ |\ \text{do}(t)\big)\quad\text{(Modularity between T and Y)}\\
&=\sum_wP\big(y\ |\ t,w\big)P\big(w\big)\quad\text{(Modularity between W and T)}\\

\end{aligned}
$$

### Relation to d-separation

We can use the backdoor adjustment if $W$ <u>d-separates $T$ from $Y$</u> in the manipulated graph.

i.e., $Y\Longrightarrow T$ is d-separates by $W$.

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
*This indicates that we simply choose $W$ so that it satisfies the backdoor criterion.*

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





















