# Toy_NK_Landscape
A basic NK landscape model based on numpy

## NK Landscape Comparison
This implementation is a less-memory deisign, leading to much more running time. In such a design, the fitness is stored by list rather than the hash dict cache.

## NK Landscape Instance
Compared to this version, we use a hash dict cache design, faster and simultaneously with higher memory occupation.

## Conclusion
The numpy design or the matrix design is not suitable. The reason is most of the calculation lie in the query of fitness number, rather than the repeatitivr operation that numpy can overperform.

Ultimately, we reach the consensus that hash dict in Python is the picked one.
