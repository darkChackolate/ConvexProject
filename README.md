This project explores three techniques: Nesterov’s
Accelerated Gradient Descent, the Heavy Ball Method,
and Conjugate Gradient Descent. The Heavy Ball Method,
introduced by Polyak in 1964, introduces a momentum term
that helps smooth the descent path and reduce oscillations.
Nesterov’s method, on the other hand, applies momentum
more judiciously by incorporating a look-ahead step, resulting
in optimal convergence rates for smooth convex problems.
Finally, Conjugate Gradient Descent, though originally de-
veloped for quadratic minimization, can be interpreted as an
acceleration of gradient descent that conjugates successive
search directions to avoid redundant traversals.
The analysis of these methods are done through the exam-
ination of three case studies:
1) Quadratic minimization with varying condition num-
bers to assess iteration complexity and sensitivity to
curvature.
2) L2-regularized logistic regression on a synthetic, lin-
early separable dataset to test convergence on a strongly
convex loss function.
3) Linear regression for vehicle price prediction using
a real-world dataset from Kaggle to evaluate practical
performance under regularization.
These examples span theoretical and practical applications,
allowing us to compare the methods under both idealized
and noisy real-world settings. The results reinforce theoretical
convergence claims and highlight when and why one method
may be preferred over another. In particular, the findings
show how Nesterov’s and Conjugate Gradient methods adapt
more effectively to structure and curvature, while the Heavy
Ball method excels in smooth quadratic cases with well-tuned
parameters.
