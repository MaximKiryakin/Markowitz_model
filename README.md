Постановка задачи

Пусть у нас есть n активов с ожидаемыми доходностями $\mu_i$, стандартными отклонениями $\sigma_i$, корреляциями $\rho_{i, j}$. Инвестиционный портфель задан весами $x_i$. Какие веса активов в портфеле минимизируют риск при фиксированной ожидаемой доходности?  
\begin{equation*}
x = 
\begin{bmatrix}
x_1 \\
x_2 \\
\vdots \\
x_n \\
\end{bmatrix}
\mu = 
\begin{bmatrix}
\mu_1 \\
\mu_2 \\
\vdots \\
\mu_n \\
\end{bmatrix}
S = 
\begin{bmatrix}
\sigma_1^2 & \rho_{1,2}\sigma_1\sigma_2 &\ldots &\rho_{1,n}\sigma_1\sigma_n \\
\rho_{2,1}\sigma_2\sigma_1 & \sigma_2^2 &\ldots &\rho_{2,n}\sigma_2\sigma_n \\
\vdots & \vdots & & \vdots\\
\rho_{n,1}\sigma_n\sigma_1 & \rho_{n,2}\sigma_n\sigma_2 &\ldots & \sigma_n^2  \\
\end{bmatrix}
\end{equation*}

Задача квадратичного программирования

\begin{equation*}
\begin{cases}
x^{T}Sx  \rightarrow min \\
\mu^Tx = r \\
\sum{x_i} = 1\\
x \ge 0
\end{cases}
\end{equation*}
