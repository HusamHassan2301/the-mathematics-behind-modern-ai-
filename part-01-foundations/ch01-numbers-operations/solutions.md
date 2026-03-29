# Chapter 1 Solutions — Short Guidance

These are not full model answers.
They are short guides to help you check your observations.

---

##  1. Scaling an Embedding

When an embedding is multiplied by a constant, every component is scaled by that same factor.

Typical observation:

* multiplying by `2` doubles all values
* multiplying by `5` increases the distance from zero even more
* multiplying by `0.1` shrinks the vector toward zero

Geometrically, scaling changes the size of the vector without changing its basic direction when the factor is positive.

---

##  2. Shifting an Embedding

When a constant is added to the embedding, every component increases or decreases by the same amount.

Typical observation:

* all values move together
* relative gaps between components stay the same
* the whole vector is translated

Geometrically, shifting moves the representation through space.

---

##  3. Combining Operations

Scaling then shifting is generally **not** the same as shifting then scaling.

This shows that operations on vectors are order-sensitive.

Typical conclusion:

* the final result depends on the sequence of operations
* transformations can interact in different ways

---

##  4. Precision Experiment

`float32` usually preserves more detail than `float16`.

Typical observation:

* some values look slightly rounded in `float16`
* differences may be small in short examples
* these differences become more important at scale

In large AI models, lower precision saves memory and speeds computation, but may introduce numerical error.

---

##  5. Weight Update Sensitivity

The update rule is:

`w_new = w - alpha * g`

Typical observation:

* very small `alpha` produces tiny changes
* very large `alpha` produces large jumps
* changing the sign of `g` changes the update direction

A learning rate that is too large can make updates unstable.

---

##  6. Visualizing an Embedding

The point moves depending on the operation:

* scaling changes its distance from the origin
* shifting translates it across the plane

This helps build intuition for how learning changes representations in space.

---

##  7. Direction of Movement

The sign of the gradient determines the direction of the update.

Typical observation:

* positive gradient moves the weight one way
* negative gradient moves it the opposite way

The gradient tells the model which direction reduces error.

---

##  8. Multiple Updates

Repeated updates show how a parameter changes over time.

Typical observation:

* with moderate values, the weight changes steadily
* with overly large updates, the value may move too fast or behave unstably

This is a simplified view of iterative learning in machine learning.

---

##  Final Task

A strong final observation should include:

* the numerical change you saw
* the operation that caused it
* the AI meaning of that change

Example:

> Scaling increased every component of the embedding, which moved the representation farther from the origin. This suggests that even simple arithmetic operations can significantly reshape how information is represented inside a model.
