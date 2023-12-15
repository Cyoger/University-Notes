11 - 13 questions
# 1 Short questions (9 - 10 points)
- Matlab commands
- Computational complexity
- Integration formula errors


# 2 System of equations/matrix
- Gaussian elimination or LU factorization
- Row interchange if partial pivoting or if pivot is 0
- No row interchange otherwise
- Cholesky factorization will not be tested


# 3 Jacobi and Gauss-Seidel method
- Linear or non-linear system
- Will converge for a linear system if the matrix A formed from the equations is strictly diagonally dominant. Otherwise it may or may not converge
- Will converge for a non-linear system if the functions and partial derivatives are continuous over a plane containing the initial guess and solution, and the sums of the magnitudes of the solutions of the partial derivatives are less than one
$|\frac{\partial g_1(sol)}{\partial x}| + |\frac{\partial g_1(sol)}{\partial y}| < 1$ and $|\frac{\partial g_2(sol)}{\partial x}| + |\frac{\partial g_2(sol)}{\partial y}| < 1$ 

- Otherwise may or may not converge

# 4 Eigenvalues and eigenvector
- Solve $|A - \lambda I| = 0$ for eigenvalues
- Solve $(A-\lambda I)\vec{x} = \vec{0}$ for eigenvectors
- Power method
Find $Y_k = AX_k$, then find $\mu_k$ is the element of $Y_k$ that has largest magnitude
e.g. if $Y_k = (1,2,-3)$, then $\mu_k = -3$
Then, $X_{k+1} = \frac{1}{\mu_k}Y_k$

Power methods converges if the magnitude of the dominant eigenvalue is unique.
If the eigenvalues are $1, -1, 5$, then the power method will converge.
If the eigenvalues are $1, -5, 5$ then the power method will not converge.

# Solving non-linear equations
- Bisection method starting from $[a,b]$:
    - $p = \frac{a+b}{2}$ 
    - If $f(a), f(p)$ have same sign, then use $[p,b]$
    - If $f(a), f(p)$ have different signs, then use $[a,p]$
- Method of false position starting from $[a,b]$
    - $p = b - \frac{f(b)(b-a)}{f(b) - f(a)}$
    - If $f(a), f(p)$ have same sign, then use $[p,b]$
    - If $f(a), f(p)$ have different signs, then use $[a,p]$
    - If $f$ is continuous on $[a,b]$ and $f(a), f(b)$ have opposite signs, then Bisection and False position will converge. 
    - Both globally convergent

- Newton's method:
    - $p_n = p_{n-1} - \frac{f(p_{n-1})}{f'(p_{n-1})}$
    - Will not ask conditions of convergence
- Secant method:
    - $p_n = P_{n-1} - \frac{f(p_{n-1})(p_{n-1} - p_{n-1})}{f(p_{n-1}) - f(p_{n-2})}$
    - $f$ is continuous on $[a,b]$

- Convergence rate of bisection and false position is linear
- Convergence rate of Newton and secant method is quadratic

- Fixed point method:
    - We need $x = g(x)$
    - $p_n = g(p_{n-1})$ iteration
    - If $g, g'$ are continuous on $[a,b]$ and the initial guess $p_0$ and the solution are in $[a,b]$
        - If $|g'(sol)| < 1$ then fixed point converges

- 2 - 3 questions from these methods

# Polynomials
- Lagrange polynomial
- Newton polynomial
    - Divided difference table


# Least squares approximation
- 1 question
- Change of variables


# Derivatives
- 1 or 2 questions
- Starting from difference table
- Find the order of error in the approximation (Taylor expansion)

# Integration
- Trapezoidal
- Simpsons
- Will not ask Simpsons 3/8
- Composite trapezoidal 
- Composite Simpsons
- 1 question 

# Numerical optimization
- Local min value of $f$
- Golden ratio searc11 - 13 questions
# 1 Short questions (9 - 10 points)
- Matlab commands
- Computational complexity
- Integration formula errors


# 2 System of equations/matrix
- Gaussian elimination or LU factorization
- Row interchange if partial pivoting or if pivot is 0
- No row interchange otherwise
- Cholesky factorization will not be tested


# 3 Jacobi and Gauss-Seidel method
- Linear or non-linear system
- Will converge for a linear system if the matrix A formed from the equations is strictly diagonally dominant. Otherwise it may or may not converge
- Will converge for a non-linear system if the functions and partial derivatives are continuous over a plane containing the initial guess and solution, and the sums of the magnitudes of the solutions of the partial derivatives are less than one
$|\frac{\partial g_1(sol)}{\partial x}| + |\frac{\partial g_1(sol)}{\partial y}| < 1$ and $|\frac{\partial g_2(sol)}{\partial x}| + |\frac{\partial g_2(sol)}{\partial y}| < 1$ 

- Otherwise may or may not converge

# 4 Eigenvalues and eigenvector
- Solve $|A - \lambda I| = 0$ for eigenvalues
- Solve $(A-\lambda I)\vec{x} = \vec{0}$ for eigenvectors
- Power method
Find $Y_k = AX_k$, then find $\mu_k$ is the element of $Y_k$ that has largest magnitude
e.g. if $Y_k = (1,2,-3)$, then $\mu_k = -3$
Then, $X_{k+1} = \frac{1}{\mu_k}Y_k$

Power methods converges if the magnitude of the dominant eigenvalue is unique.
If the eigenvalues are $1, -1, 5$, then the power method will converge.
If the eigenvalues are $1, -5, 5$ then the power method will not converge.

# Solving non-linear equations
- Bisection method starting from $[a,b]$:
    - $p = \frac{a+b}{2}$ 
    - If $f(a), f(p)$ have same sign, then use $[p,b]$
    - If $f(a), f(p)$ have different signs, then use $[a,p]$
- Method of false position starting from $[a,b]$
    - $p = b - \frac{f(b)(b-a)}{f(b) - f(a)}$
    - If $f(a), f(p)$ have same sign, then use $[p,b]$
    - If $f(a), f(p)$ have different signs, then use $[a,p]$
    - If $f$ is continuous on $[a,b]$ and $f(a), f(b)$ have opposite signs, then Bisection and False position will converge. 
    - Both globally convergent

- Newton's method:
    - $p_n = p_{n-1} - \frac{f(p_{n-1})}{f'(p_{n-1})}$
    - Will not ask conditions of convergence
- Secant method:
    - $p_n = P_{n-1} - \frac{f(p_{n-1})(p_{n-1} - p_{n-1})}{f(p_{n-1}) - f(p_{n-2})}$
    - $f$ is continuous on $[a,b]$

- Convergence rate of bisection and false position is linear
- Convergence rate of Newton and secant method is quadratic

- Fixed point method:
    - We need $x = g(x)$
    - $p_n = g(p_{n-1})$ iteration
    - If $g, g'$ are continuous on $[a,b]$ and the initial guess $p_0$ and the solution are in $[a,b]$
        - If $|g'(sol)| < 1$ then fixed point converges

- 2 - 3 questions from these methods

# Polynomials
- Lagrange polynomial
- Newton polynomial
    - Divided difference table


# Least squares approximation
- 1 question
- Change of variables


# Derivatives
- 1 or 2 questions
- Starting from difference table
- Find the order of error in the approximation (Taylor expansion)

# Integration
- Trapezoidal
- Simpsons
- Will not ask Simpsons 3/8
- Composite trapezoidal 
- Composite Simpsons
- 1 question 

# Numerical optimization
- Local min value of $f$
- Golden ratio search method


11 - 13 questions
# 1 Short questions (9 - 10 points)
- Matlab commands
- Computational complexity
- Integration formula errors


# 2 System of equations/matrix
- Gaussian elimination or LU factorization
- Row interchange if partial pivoting or if pivot is 0
- No row interchange otherwise
- Cholesky factorization will not be tested


# 3 Jacobi and Gauss-Seidel method
- Linear or non-linear system
- Will converge for a linear system if the matrix A formed from the equations is strictly diagonally dominant. Otherwise it may or may not converge
- Will converge for a non-linear system if the functions and partial derivatives are continuous over a plane containing the initial guess and solution, and the sums of the magnitudes of the solutions of the partial derivatives are less than one
$|\frac{\partial g_1(sol)}{\partial x}| + |\frac{\partial g_1(sol)}{\partial y}| < 1$ and $|\frac{\partial g_2(sol)}{\partial x}| + |\frac{\partial g_2(sol)}{\partial y}| < 1$ 

- Otherwise may or may not converge

# 4 Eigenvalues and eigenvector
- Solve $|A - \lambda I| = 0$ for eigenvalues
- Solve $(A-\lambda I)\vec{x} = \vec{0}$ for eigenvectors
- Power method
Find $Y_k = AX_k$, then find $\mu_k$ is the element of $Y_k$ that has largest magnitude
e.g. if $Y_k = (1,2,-3)$, then $\mu_k = -3$
Then, $X_{k+1} = \frac{1}{\mu_k}Y_k$

Power methods converges if the magnitude of the dominant eigenvalue is unique.
If the eigenvalues are $1, -1, 5$, then the power method will converge.
If the eigenvalues are $1, -5, 5$ then the power method will not converge.

# Solving non-linear equations
- Bisection method starting from $[a,b]$:
    - $p = \frac{a+b}{2}$ 
    - If $f(a), f(p)$ have same sign, then use $[p,b]$
    - If $f(a), f(p)$ have different signs, then use $[a,p]$
- Method of false position starting from $[a,b]$
    - $p = b - \frac{f(b)(b-a)}{f(b) - f(a)}$
    - If $f(a), f(p)$ have same sign, then use $[p,b]$
    - If $f(a), f(p)$ have different signs, then use $[a,p]$
    - If $f$ is continuous on $[a,b]$ and $f(a), f(b)$ have opposite signs, then Bisection and False position will converge. 
    - Both globally convergent

- Newton's method:
    - $p_n = p_{n-1} - \frac{f(p_{n-1})}{f'(p_{n-1})}$
    - Will not ask conditions of convergence
- Secant method:
    - $p_n = P_{n-1} - \frac{f(p_{n-1})(p_{n-1} - p_{n-1})}{f(p_{n-1}) - f(p_{n-2})}$
    - $f$ is continuous on $[a,b]$

- Convergence rate of bisection and false position is linear
- Convergence rate of Newton and secant method is quadratic

- Fixed point method:
    - We need $x = g(x)$
    - $p_n = g(p_{n-1})$ iteration
    - If $g, g'$ are continuous on $[a,b]$ and the initial guess $p_0$ and the solution are in $[a,b]$
        - If $|g'(sol)| < 1$ then fixed point converges

- 2 - 3 questions from these methods

# Polynomials
- Lagrange polynomial
- Newton polynomial
    - Divided difference table


# Least squares approximation
- 1 question
- Change of variables


# Derivatives
- 1 or 2 questions
- Starting from difference table
- Find the order of error in the approximation (Taylor expansion)

# Integration
- Trapezoidal
- Simpsons
- Will not ask Simpsons 3/8
- Composite trapezoidal 
- Composite Simpsons
- 1 question 

# Numerical optimization
- Local min value of $f$
- Golden ratio searc11 - 13 questions
# 1 Short questions (9 - 10 points)
- Matlab commands
- Computational complexity
- Integration formula errors


# 2 System of equations/matrix
- Gaussian elimination or LU factorization
- Row interchange if partial pivoting or if pivot is 0
- No row interchange otherwise
- Cholesky factorization will not be tested


# 3 Jacobi and Gauss-Seidel method
- Linear or non-linear system
- Will converge for a linear system if the matrix A formed from the equations is strictly diagonally dominant. Otherwise it may or may not converge
- Will converge for a non-linear system if the functions and partial derivatives are continuous over a plane containing the initial guess and solution, and the sums of the magnitudes of the solutions of the partial derivatives are less than one
$|\frac{\partial g_1(sol)}{\partial x}| + |\frac{\partial g_1(sol)}{\partial y}| < 1$ and $|\frac{\partial g_2(sol)}{\partial x}| + |\frac{\partial g_2(sol)}{\partial y}| < 1$ 

- Otherwise may or may not converge

# 4 Eigenvalues and eigenvector
- Solve $|A - \lambda I| = 0$ for eigenvalues
- Solve $(A-\lambda I)\vec{x} = \vec{0}$ for eigenvectors
- Power method
Find $Y_k = AX_k$, then find $\mu_k$ is the element of $Y_k$ that has largest magnitude
e.g. if $Y_k = (1,2,-3)$, then $\mu_k = -3$
Then, $X_{k+1} = \frac{1}{\mu_k}Y_k$

Power methods converges if the magnitude of the dominant eigenvalue is unique.
If the eigenvalues are $1, -1, 5$, then the power method will converge.
If the eigenvalues are $1, -5, 5$ then the power method will not converge.

# Solving non-linear equations
- Bisection method starting from $[a,b]$:
    - $p = \frac{a+b}{2}$ 
    - If $f(a), f(p)$ have same sign, then use $[p,b]$
    - If $f(a), f(p)$ have different signs, then use $[a,p]$
- Method of false position starting from $[a,b]$
    - $p = b - \frac{f(b)(b-a)}{f(b) - f(a)}$
    - If $f(a), f(p)$ have same sign, then use $[p,b]$
    - If $f(a), f(p)$ have different signs, then use $[a,p]$
    - If $f$ is continuous on $[a,b]$ and $f(a), f(b)$ have opposite signs, then Bisection and False position will converge. 
    - Both globally convergent

- Newton's method:
    - $p_n = p_{n-1} - \frac{f(p_{n-1})}{f'(p_{n-1})}$
    - Will not ask conditions of convergence
- Secant method:
    - $p_n = P_{n-1} - \frac{f(p_{n-1})(p_{n-1} - p_{n-1})}{f(p_{n-1}) - f(p_{n-2})}$
    - $f$ is continuous on $[a,b]$

- Convergence rate of bisection and false position is linear
- Convergence rate of Newton and secant method is quadratic

- Fixed point method:
    - We need $x = g(x)$
    - $p_n = g(p_{n-1})$ iteration
    - If $g, g'$ are continuous on $[a,b]$ and the initial guess $p_0$ and the solution are in $[a,b]$
        - If $|g'(sol)| < 1$ then fixed point converges

- 2 - 3 questions from these methods

# Polynomials
- Lagrange polynomial
- Newton polynomial
    - Divided difference table


# Least squares approximation
- 1 question
- Change of variables


# Derivatives
- 1 or 2 questions
- Starting from difference table
- Find the order of error in the approximation (Taylor expansion)

# Integration
- Trapezoidal
- Simpsons
- Will not ask Simpsons 3/8
- Composite trapezoidal 
- Composite Simpsons
- 1 question 

# Numerical optimization
- Local min value of $f$
- Golden ratio search method


