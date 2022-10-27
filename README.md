# minimize ComfortLoss

one building including N floors

DR demand: reduce energy consumption by $DR_{demand}$ kWh in T hours

------

objective function:

$\min \sum_{i=1}^{N} \sum_{t=1}^{T}Population_i^t \times |\Delta PMV_i^t|$

constraints:

$\sum_{i=1}^N \sum_{t=1}^T DR_i^t \ge DR_{demand}$

$-3 \le \Delta Tset_i^t \le 3$

decision variables:

$\Delta Tset$ is a matrix of shape (N,T)

------

$DR_i^t=f_1(\Delta Tset_i^t,\ Population_i^t,\ to^t)$

$\Delta PMV_i^t = f_2(\Delta Tset_i^t)$

ziliangwei
