# Toy_NK_Landscape
A basic NK landscape model based on numpy

## NK Landscape Comparison
This is a less-memory design, resulting in a much longer running time. Fitness values are stored by list rather than a hash dict.
## NK Landscape Instance
We also use a hash dict cache design, which is faster and occupies more memory.

## Conclusion
Neither the numpy design nor the matrix design are appropriate. This is because most of the work is done by querying the fitness number, rather than by repeating repetitive operations that numpy can speed up. As a result, the exchange between the original Python environment and the Numpy environment causes more cost than benefit.

In the end, we decide that Python's hash dict is the best.
