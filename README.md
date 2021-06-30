# Global Optimizer Scoring

Global optimizer scoring implementation in C++ to find approximately globally optimized scoring w for the MSE E{0.5||y-f(x|w)||^2} error function.

The software discretizes data to 0/1 indicator variables and then datamines frequent sets and their subsets which are used as variables for "linear" scoring.

The linear problem is solved by calculating pseudoinverse of the correlation matrix for the linear problem y=w^t*x + b. The trick is that with linearized 
problem we only have one optimum and it is the global optimum of the problem.

Tomas Ukkonen
tomas.ukkonen@novelinsight.fi

