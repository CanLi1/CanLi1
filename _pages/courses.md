---
title: "Li Group - Courses"
layout: textlay
excerpt: "Courses"
sitemap: false
permalink: /courses
---

## CHE697 Computational Optimization, Spring 2024

**Instructor:** Can Li 
**Email:** canli@purdue.edu

---

### Course Description:
This is a graduate-level introductory course to mathematical optimization. We will cover the theory and algorithms of linear programming, mixed-integer linear/nonlinear programming, conic programming, global optimization of nonconvex problems, and decomposition algorithms for mixed-integer programs. Special focus will be given to using the APIs of modern computational software including CPLEX, Gurobi, Mosek, Pytorch with implementations in Python. We will motivate the algorithms using modern applications in chemical engineering, transportation, energy systems, machine learning, and control.

The course lectures will be 30% proofs, 50% algorithms and computation, and 20% modeling and applications in engineering. The homework will keep a similar portion. However, we will not have proofs in the exams since this is a class targeted at engineering students. 

### Topics Covered (tentative)
#### Optimization basics
- Convex sets, functions
- Unconstrained optimization, gradient descent, Newton's method
- Simple applications of optimization models
- Modeling using pyomo

#### Linear and conic programming
- Applications
- Basics of polyhedral theory, LP duality
- Second-order cone programming (SOCP)
- Semidefinite programming (SDP), Goemans-Williamson

#### Nonlinear programming
- Applications
- Optimality conditions
- Barrier algorithm, interior point algorithm

#### (Mixed)-integer linear programming
- Modeling of discrete and continuous decisions
- Propositional logic, modeling of disjunctions
- Applications
- Branch and bound
- Cutting planes
- Disjunctive programming


#### Global optimization of nonconvex problems
- Applications
- Convex relaxations, McCormick Inequality
- Spatial branch and bound
- Mixed-integer nonlinear programming

#### Decomposition algorithms
- Benders decomposition, stochastic programming
- Dantzig Wolfe decomposition, column generation, vehicle routing problems
- Lagrangian decomposition
- ADMM 

#### Advanced topics on computation
- Numerical linear algebra
- Advanced solver callbacks
- Parallel computing
- GPU computing

### Recommended Textbooks:
This class will not exactly follow any textbook. But we may cover some of the content in the following textbooks.
1. Grossmann, I. E. (2021). Advanced optimization for process systems engineering. Cambridge University Press.
2. Wolsey, L. A. (2020). Integer programming. John Wiley & Sons.
3. Bertsimas, D., & Tsitsiklis, J. N. (1997). Introduction to linear optimization (Vol. 6, pp. 479-530). Belmont, MA: Athena scientific.
4. Ben-Tal, A., & Nemirovski, A. (2001). Lectures on modern convex optimization: analysis, algorithms, and engineering applications. Society for industrial and applied mathematics.
5. Conforti, M., Cornuéjols, G., Zambelli, G., Conforti, M., Cornuéjols, G., & Zambelli, G. (2014). Integer programming models (pp. 45-84). Springer International Publishing.

### Software
We will use the following software 
- [Pyomo](https://www.pyomo.org/) is a collection of Python software packages for formulating optimization models. Tutorial: [ND Pyomo Cookbook](https://jckantor.github.io/ND-Pyomo-Cookbook/README.html)
- [Gurobi](https://www.gurobi.com/documentation/) and [Cplex](https://www.ibm.com/products/ilog-cplex-optimization-studio) are both high-performance mathematical programming solver for linear programming, mixed integer programming, and quadratic programming.
- [Mosek](https://www.mosek.com/) is a software package for the solution of linear, mixed-integer linear, quadratic, mixed-integer quadratic, quadratically constraint, conic and convex nonlinear mathematical optimization problems.

### Prerequisite

Some familiarity with linear algebra, calculus, and programming in python is required.
- YouTube videos review of linear algebra and calculus by [3Blue1Brown](https://www.youtube.com/@3blue1brown/courses)
- [Linear algebra review](https://www.cs.cmu.edu/~zkolter/course/linalg/index.html)  videos by Zico Kolter
- General mathematical review: Appendix A of  [Boyd and Vandenberghe (2004)](https://web.stanford.edu/~boyd/cvxbook/bv_cvxbook.pdf)

### Related courses
- [Convex optimization](https://www.stat.cmu.edu/~ryantibs/convexopt/) by Ryan Tibshirani 
- [Convex analysis](https://ocw.mit.edu/courses/6-253-convex-analysis-and-optimization-spring-2012/pages/syllabus/) by Dimitri Bertsekas
- [Linear programming](https://www2.isye.gatech.edu/~sdey30/CourseLinearProgramming.html) by Santanu Dey
- [Integer programming](https://coral.ise.lehigh.edu/~ted/teaching/ie418/) by Ted Ralphs
- [Linear and convex optimization classes](https://www2.isye.gatech.edu/~nemirovs/) by Arkadi Nemirovski

**Last updated:** October 12, 2023
<br /><br /><br /><br /><br /><br /><br /><br />