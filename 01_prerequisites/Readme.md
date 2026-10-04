## The prerequisites were selected first by attending the course, then by using a top down approach to find the core I will work on.

The result of this top down approach is handwritten in the pdf named "Top_Down", here is a summary of it :


## Learning path overview

| Block | Topic | Unlocks |
|:-----:|-------|---------|
| 0 | Logical foundations | Rigorous reading of every later definition |
| 1 | Linear algebra | ℝⁿ, constraints, linear programs |
| 2 | Single-variable real analysis | Limits, continuity, derivatives, Taylor |
| 3 | Euclidean geometry & quadratic forms | Hessian criteria, mean-variance |
| 4 | Metric spaces & topology | Existence of optima (compactness) |
| 5 | Multivariable differential calculus | Gradient, Hessian, optimality conditions |
| 6 | Convexity | Local = global, uniqueness |
| 7 | Unconstrained & equality-constrained optimization | Critical points, Lagrange multipliers |
| 8 | Linear programming | Simplex, duality, KKT |
| 9 | Iterative methods & numerical solvers | Gradient descent, Newton, Excel Solver |
| 10 | Probability, statistics & portfolio selection | Mean-variance portfolio |
| 11 | Combinatorics & combinatorial optimization | Integer programming, graphs, complexity |

---

## Block 0 — Logical foundations

- [ ] Logic: logical connectives, quantifiers ∀ and ∃, abstract reasoning
- [ ] Elementary set theory: subsets, finite intersections, arbitrary unions, complements, indexed families of sets
- [ ] Maps between sets f : E → F: direct image, inverse image
- [ ] Cardinality: countable and uncountable sets (*"Infinity and infinity"*). Light coverage is enough, since it has little direct use in optimization

## Block 1 — Linear algebra

- [ ] Vector spaces, linear combinations, ℝⁿ as a state or decision space
- [ ] Matrix calculus, systems of linear equations, image and kernel
- [ ] Endomorphisms, invertibility, determinant
- [ ] Affine algebra: affine spaces, segments, convex combinations, barycenters

## Block 2 — Single-variable real analysis

- [ ] Numerical sequences, convergence, limits, accumulation points
- [ ] Continuity on ℝ, inequalities
- [ ] Derivatives: slope, link with monotonicity, classes C⁰, C¹, C² and Cᵏ
- [ ] Taylor expansion in one variable, remainder and local approximation

## Block 3 — Euclidean geometry & quadratic forms

- [ ] Inner product, norms, balls, projections
- [ ] Symmetric matrices, quadratic forms, positive (semi-)definite matrices

## Block 4 — Metric spaces & topology

- [ ] Distance d : X × X → [0, +∞[, metric spaces, normed vector spaces, sequence and function spaces
- [ ] Balls, open and closed sets, dense subsets
- [ ] General topology: bases, induced topology. A topology can be defined without a distance, and metric spaces are a special case
- [ ] Topological continuity, homeomorphisms, uniform continuity
- [ ] Compactness, connectedness, separability, semi-continuity. These are what guarantee that an optimum exists

## Block 5 — Multivariable differential calculus

- [ ] Multivariable differentiability, classes C⁰, C¹ and C² in several variables
- [ ] The gradient as a linear map
- [ ] The Hessian as the matrix of second derivatives, and the quadratic form associated with it
- [ ] Multivariable Taylor expansion, remainder and local approximation

## Block 6 — Convexity

*"Why convexity is the whole game"*

- [ ] Convex sets: definition and properties, convex polyhedra and polytopes, extreme points
- [ ] Convex functions: convexity inequality, epigraph, sublevel sets
- [ ] Differential characterizations: increasing derivative, positive semi-definite Hessian, and a positive definite Hessian as a sufficient condition for strict convexity
- [ ] Why it matters: every local minimum is global, and existence and uniqueness follow

## Block 7 — Unconstrained & equality-constrained optimization

- [ ] Critical points (∇f(x) = 0)
- [ ] First- and second-order optimality conditions
- [ ] Existence and uniqueness of a minimizer
- [ ] Convexity as a guarantee of global optimality
- [ ] One equality constraint: local constraint manifold, feasible directions
- [ ] Lagrange multiplier, second-order conditions under constraint
- [ ] Link with space-reduction methods

## Block 8 — Linear programming

- [ ] Modelling with linear equations and inequalities
- [ ] Geometric view: optimizing a linear function over a convex set defined by affine inequalities
- [ ] Algorithmic linear algebra (simplex): bases, basic solutions, pivots, variable exchange, degeneracy, degenerate bases, multiple optima
  - How do you move from one basis to another?
  - What is a feasible basis?
  - When is a basis degenerate?
  - Why can degeneracy disrupt an algorithm?
  - How do you interpret a basic solution?
- [ ] Duality and optimality conditions
- [ ] KKT conditions and multipliers

## Block 9 — Iterative methods & numerical solvers

- [ ] Convergence of iterative algorithms, descent directions
- [ ] Step size selection: line search, backtracking
- [ ] Gradient descent: convergence when f is convex with a Lipschitz gradient, the non-smooth case
- [ ] Newton's method: second-order Taylor expansion, invertible Hessian, local convexity and positive definite Hessian, fast local convergence, backtracking and robustness
- [ ] Local vs global convergence, including for methods using Lagrange multipliers
- [ ] Numerical solvers (Excel Solver):
  - tolerance, convergence, precision
  - local vs global solutions
  - choice of solving method (linear, nonlinear, quadratic, integer)
  - correct formulation in a spreadsheet
  - sensitivity analysis
  - interpretation of multipliers and slack constraints

## Block 10 — Probability, statistics & portfolio selection

- [ ] Probability: expectation, variance, covariance, first- and second-order moments, covariance matrix, distributional assumptions
- [ ] Statistics: parameter estimation and uncertainty
- [ ] Portfolio selection as a linear program, portfolio constraints
- [ ] Quadratic optimization under linear constraints: minimizing portfolio variance subject to a target expected return
- [ ] Mean-variance portfolio and the convexity of the problem
- [ ] Link between convexity and optimality conditions in the mean-variance problem
- [ ] Sensitivity to estimated parameters
- [ ] Financial interpretation of risk and return

## Block 11 — Combinatorics & combinatorial optimization

- [ ] Counting applied to combinatorics: counting solutions, size of the configuration set, permutations and combinations
- [ ] Discrete variables and integer programming
- [ ] Convex relaxation and integrality gap
- [ ] Graph theory: graphs, vertices, edges, weights, paths, cycles, trees, flows, capacities
- [ ] Algorithmic complexity:
  - problems solvable in polynomial time
  - NP-hard problems
  - heuristics and metaheuristics
  - approximation guarantees

---

## Traceability to the course chapters

The blocks reorganize the whiteboard items by dependency. This table maps every item from course parts II, III and IV to the blocks that cover its prerequisites.

| # | Course item | Part | Blocks |
|:-:|-------------|:----:|:------:|
| 1 | ℝⁿ and matrix calculus | II | 1 |
| 2 | Infinity and infinity | II | 0 |
| 3 | Metric spaces | II | 3, 4 |
| 4 | Topology | II | 4 |
| 5 | Convex sets | II | 1, 6 |
| 6 | Convex functions | II | 2, 3, 6 |
| 7 | Linear programming | III | 1, 6, 8 |
| 8 | Excel Solver | III | 9 |
| 9 | Portfolio selection (LP) | III | 3, 10 |
| 10 | Combinatorial optimization | III | 0, 11 |
| 11 | Gradient and Newton methods | IV | 5, 9 |
| 12 | Smoothness and Taylor expansion | IV | 2, 5 |
| 13 | Gradient and Hessian | IV | 3, 5, 7 |
| 14 | Unconstrained optimization | IV | 6, 7 |
| 15 | Descent method | IV | 2, 9 |
| 16 | Newton's method | IV | 5, 9 |
| 17 | One equality constraint (Lagrangian) | IV | 7 |
| 18 | Mean-variance portfolio | IV | 3, 6, 10 |

Part IV marks the shift from a world where solutions are geometric and finite (LP, simplex, combinatorics) to one built on differentiable functions, local approximations, optimality conditions, iterative methods and nonlinear financial models.