Recurrence for divide-and-conquer
$$
T(n) = \begin{cases}
   \Theta(1) &\text{if } n<c \\
   aT(n/b)+D(n)+C(n) &\text{otherwise }
\end{cases}
$$