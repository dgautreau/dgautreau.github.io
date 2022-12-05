# Portfolio

---

### Natural Language Processing with Machine Learning

[![Open Notebook](https://img.shields.io/badge/Jupyter-Open_Notebook-yellowgreen?logo=Jupyter)](projects/ames-house-price.html)
[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-yellowgreen?logo=GitHub)](https://github.com/chriskhanhtran/kaggle-house-price/blob/master/ames-house-price.ipynb)

<div style="text-align: justify">The release of Google's BERT is described as the beginning of a new era in NLP. In this notebook I'll use the HuggingFace's transformers library to fine-tune pretrained BERT model for a classification task. Then I will compare BERT's performance with a baseline model, in which I use a TF-IDF vectorizer and a Naive Bayes classifier. The transformers library helps us quickly and efficiently fine-tune the state-of-the-art BERT model and yield an accuracy rate 10% higher than the baseline model.</div>

<center><img src="images/dummy_thumbnail.jpg"/></center>

---

### Detect Non-negative Airline Tweets: BERT for Sentiment Analysis

[![Open Notebook](https://img.shields.io/badge/Jupyter-Open_Notebook-yellowgreen?logo=Jupyter)](projects/ames-house-price.html)
[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-yellowgreen?logo=GitHub)](https://github.com/chriskhanhtran/kaggle-house-price/blob/master/ames-house-price.ipynb)

<div style="text-align: justify">The release of Google's BERT is described as the beginning of a new era in NLP. In this notebook I'll use the HuggingFace's transformers library to fine-tune pretrained BERT model for a classification task. Then I will compare BERT's performance with a baseline model, in which I use a TF-IDF vectorizer and a Naive Bayes classifier. The transformers library helps us quickly and efficiently fine-tune the state-of-the-art BERT model and yield an accuracy rate 10% higher than the baseline model.</div>

<center><img src="images/dummy_thumbnail.jpg"/></center>

---

### Calculating Magnetic Exchanges from Linear Regression and Density Functional Theory

[![Open Notebook](https://img.shields.io/badge/Jupyter-Open_Notebook-yellowgreen?logo=Jupyter)](projects/ames-house-price.html)
[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-yellowgreen?logo=GitHub)](https://github.com/chriskhanhtran/kaggle-house-price/blob/master/ames-house-price.ipynb)

I used this approach in the following publications:
<ul>
  <li><a href="https://arxiv.org/abs/2105.06695">Uniaxial strain control of bulk ferromagnetism in rare-earth titanates</a></li>
  <li><a href="https://arxiv.org/abs/2102.01542">First-principles characterization of the magnetic properties of \(Cu_2(OH)_3Br\) </a></li>
  <li><a href="https://arxiv.org/abs/2006.10922">Coexistence and interaction of spinons and magnons in an antiferromagnet with alternating antiferromagnetic and ferromagnetic quantum spin chains</a></li>
</ul>

<div style="text-align: justify">


  Using spin-polarized denisty functional theory (DFT) calculations, one can extract magnetic exchange constants as follows: after calculating the energy of different spin configurations using spin-DFT, use linear regression to fit the energies to a classical Heisenberg Hamiltonian, \(H = E_0\frac{1}{2}\sum_{ij}J_{ij} \textbf{S}_i \cdot \textbf{S}_j\). Each spin configuration will have an associated equation, determined by the particular \(\textbf{S}_i \cdot \textbf{S}_j\) terms. If we have \(N\) spin configurations, then we have \(N\) corresponding equations, which can be condensed into matrix form as follows:

$$
\begin{pmatrix}
E_1  \\
E_2  \\
\vdots \\
E_N
\end{pmatrix} = \begin{pmatrix}
1 & \beta_{11} & \beta_{12} & \dots & \beta_{1m}\\
1 & \beta_{21} & \beta_{22} & \dots & \beta_{2m}\\
\vdots & \vdots & \vdots & \ddots & \vdots\\
1 & \beta_{N1} & \beta_{N2} & \dots & \beta_{Nm}\\
\end{pmatrix}
\begin{pmatrix}
E_0 \\
J_1 \\
J_2 \\
\vdots\\
J_m
\end{pmatrix}
$$


where \(\beta_{ij}\) is the coefficient of \(J_j\) for spin configuration $i$. In practice the right and left-hand sides are not equal. We do not know the values for the set of exchanges \(J\) and the paramagnetic energy \(E_0\). We can only try to find the set of values which minimizes a measure of the difference in the RHS and LHS. As such, we define a cost function \(\Theta\)

$$
\Theta = 
\begin{Vmatrix}
\begin{pmatrix}E_1  \\
E_2  \\
\vdots \\
E_N
\end{pmatrix} - \begin{pmatrix}
1 & \beta_{11} & \beta_{12} & \dots & \beta_{1m}\\
1 & \beta_{21} & \beta_{22} & \dots & \beta_{2m}\\
\vdots & \vdots & \vdots & \ddots & \vdots\\
1 & \beta_{N1} & \beta_{N2} & \dots & \beta_{Nm}\\
\end{pmatrix}
\begin{pmatrix}
E_0 \\
J_1 \\
J_2 \\
\vdots\\
J_m
\end{pmatrix} 
\end{Vmatrix}^2
$$

for which the optimal parameters of our model, \(E_0\), \(J_1\), ..., are obtained when \(\Theta\) is minimized.</div>
<br>
<center><img src="images/dummy_thumbnail.jpg"/></center>
<br>





---
---

