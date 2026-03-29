# Chapter 1 Exercises — Experiments and Exploration

These exercises are designed to be completed using the notebooks:

* [NumPy Notebook](./ch01_numpy.ipynb)
* [PyTorch Notebook](./ch01_pytorch.ipynb)

Change values. Run code. Observe behavior.

---

## 1. Scaling an Embedding

Open the NumPy notebook and go to the section on operations.

Modify the embedding by multiplying it by:

* 2
* 5
* 0.1

Observe:

* how each component changes
* how the overall structure changes

Write a short note describing what scaling does geometrically.

---

## 2. Shifting an Embedding

In the NumPy notebook, add a constant value to the embedding.

Try:

* `+1`
* `-2`
* `+10`

Observe:

* how all values move
* whether the relative differences between components change

Write a short note describing what shifting means geometrically.

---

##  3. Combining Operations

Apply both scaling and shifting to the same embedding.

Try:

* scaling first, then shifting
* shifting first, then scaling

Compare the results.

Are they the same?
What does this tell you about operations on vectors?

---

##  4. Precision Experiment

In the NumPy notebook, convert the same embedding into:

* `float32`
* `float16`

Print both arrays and compare them.

Observe:

* where rounding appears
* whether all values remain identical
* how precision changes the stored representation

Write a short note on why this matters in large AI models.

---

##  5. Weight Update Sensitivity

In the weight update section, modify:

* the learning rate `alpha`
* the gradient `g`

Try:

* very small `alpha` such as `0.0001`
* very large `alpha` such as `1.0`
* positive and negative gradient values

Observe:

* how much the weight changes
* when the update becomes very small
* when the update becomes unstable or too aggressive

---

##  6. Visualizing an Embedding

Take the first two dimensions of an embedding and plot them as a point in 2D space.

Then:

* plot the original point
* apply scaling and plot again
* apply shifting and plot again

Describe how the point moves.

---

##  7. Direction of Movement

Change the sign of the gradient in the weight update rule.

Try:

* positive gradient
* negative gradient

Observe how the updated weight changes direction.

Write a short note explaining what determines the direction of movement.

---

##  8. Multiple Updates

Repeat the weight update several times in a loop.

Try 5 to 10 updates using the same learning rate and gradient.

Observe:

* how the weight evolves over time
* whether the change is steady
* whether the value diverges or stabilizes

---

##  Final Task

Choose one experiment above and write a short observation covering:

* what changed
* why it changed
* what this suggests about AI systems
