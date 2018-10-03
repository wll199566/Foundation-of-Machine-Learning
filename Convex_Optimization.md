#  Review of Convex Optimization

## Basics

1. Concepts:
   - convex set
   - convex hull
   - convex function
   - Jensen's inequality

2. How to determine a function $ f$ is a convex function
   * if $f$ is twice differentiable, then check $\forall \mathbf{x} \in \text{dom}(f), \nabla^{2}f(x)\succeq0$.
   * if $f$ is differentiable, then check $\forall \mathbf{x, y}\in \text{dom}(f), f(\mathbf{y})-f(\mathbf{x})\geq\nabla f(\mathbf {x})(\mathbf{y}-\mathbf{x})$.
   * otherwise, use the definition of convexity: for all $\mathbf{x,y}\in \mathcal{X}$ and $\alpha \in [0,1]$, $f(\alpha \mathbf{x}+(1-\alpha)\mathbf{y}) \leq \alpha f(\mathbf{x})+(1-\alpha)f(\mathbf{y})$.
   * for composition functions , use the compositional rules provided in the text to determine the convexity of the entire function. 

## Constrained Optimization

1. Lagrangian function and its dual function
   * dual function is the infimum of Lagrangian function with respect to $\mathbf{x} \in \mathcal{X}$. 

2. Primal and its Dual Problem

   - Primal function is **minimized** w.r.t. the original variable $\mathbf{x} \in \mathcal{X} $. Dual function is **maximized** w.r.t. the dual variable $\mathbf{\alpha} \geq 0$.
   - the optimal value of dual problem is the infimum of that of primal problem, which is $d^{*} \leq p^{*}$.
   - Note that in the primal problem has no assumption about the convexity of $f, g$.

3. How to determine whether the duality gap is zero

   * if $f, g$ are convex and differentiable, then use KKT condition.

   * if $g$ are affine, then use the weak Slater's condition.

   * otherwise, use the strong Slater condition.








