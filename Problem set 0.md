# **Problem set 0**
## 1.Gradients and Hessians
*(a)* $f(x)=\frac{1}{2}x^TAx+b^Tx$,where $A$ is a symmetric matrix and $b\in\mathbb R^n$ is a vector.What is $\bigtriangledown f(x)$?  
A: $\nabla f(x) = \frac{\partial f(x)}{\partial x} = Ax + b^T$ 

*(b)* $f(x) = g(h(x))$. What is $\nabla f(x)$?  
A: $\nabla f(x) = \frac{\partial g}{\partial h}\frac{\partial h(x)}{\partial x}$

*(c)* $f(x) =\frac{1}{2}x^TAx+b^Tx$ What is the $\nabla^2 f(x)$?  
A:  $\nabla^2 f(x) = A$

*(d)* $f(x) = g(a^Tx)$, What are $\nabla f(x)$ and $\nabla^2 f(x)$ ?  
A: $\nabla f(x) = \frac{\partial g}{\partial a^Tx}a^T$ and $\nabla^2 f(x) = g^{''}(a^Tx)aa^T$

## 2. Positive definite matrices
*Definition of PSD(postive semi-definite)* : $A\ge 0, A=A^T$ and $x^TAx\ge 0$ for all $x \in \mathbb R^n$  
*Definition of PD(postive definite)*:  $A> 0, A=A^T$ and $x^TAx> 0$ for all $x \ne 0$ in other words, $x$ is a non-zero vector.The simplest example of a positive definite matrix is
the identity $I$  
*(a)* $z \in \mathbb R^n$. Show that $A = zz^T$ is PSD.  
A: $z^TAz=z^Tzz^Tz=A^TA$. It is easy to know that $A^TA \ge 0$. So $A=zz^T$ is PSD.

*(b)* $z \in \mathbb R^n$ be a non-zero vector and $A = zz^T$. What is null-space of $A$ and its rank?  
A: $N(A) = \lbrace x\in \mathbb R^n, x^Tz = 0 \rbrace , R(A)=R(zz^T)=1$ 

*(c)* $A$ is PSD and $B \in \mathbb R^n $ be arbitrary. Is $BAB^T$ PSD?  
A: $xBAB^Tx^T = (xB)A(B^Tx^T)$ since $A$ is PSD so we can get $(xB)A(B^Tx^T) \ge 0$ , $BAB^T$ is PSD.
