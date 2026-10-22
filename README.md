# $Meta-I$

#### Background
Meta-I is a measure of metacognitive sensitivity as proposed by Dayan (2023). It is the mutual information between accuracy of the choice and the confidence in that choice expressed in bits.
Metacognitive sensitivity is tied to the ability to reflect accuracy in the confidence rating about that choice, so ideally confidence should be higher for correct and lower for incorrect choices.

Meta-I quantifies how much the confidence ratings reduces of the **uncertainty about accuracy** using mutual information:
$$\text{meta-I} = H_2(r) - H_2(r \mid c)$$

in which $H_2(r)$ is the entropy of the accuracy, and $H_2(r\mid c)$ is the remaining entropy about accuracy after seeing the confidence rating $c$. Meta-I is 0, when the confidence tells us nothing about accuracy and approaches $H_2(r)$, the more confidence predicts accuracy.



Dayan additionally proposed two types of metacognitive efficiency:

 - **Meta-Ir1** = $meta-I / meta-I(d′)$: mutual information is normalized by the mutual information a naive Baysian observer would produce idealy given a certain d' (type 1 SDT perceptual sensitivity).

 - **Meta-Ir2** = $meta-I / H₂(r)$: mutual information is normalized by $H_2(r)$ the total uncertainty there is about accuracy in the first place (theoretical upper bound of meta-I).