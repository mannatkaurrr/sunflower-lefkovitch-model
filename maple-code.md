# Maple Code

## [A6] Maple sample code of modelling the seed density on a sunflower's disc using the golden ratio along with diameter

```matlab
phi = (sqrt(5)-1)/2; % = 0.6180339887499

n = -----;

rho = (0:n-1).^phi;
theta = (0:n-1)*2*pi*phi;

polar(theta, rho, 'b.');
title([num2str(n) ' Sunflower Seeds']);
set(gcf, 'color', 'w');
```

## Full Maple Code

```text
# Model Initialization and Parameters
restart:
with(LinearAlgebra):
with(MTM):

# Parameters of Population A
p1 := 0;      p2 := 9.7;    p3 := 38.8;   p4 := 87.3;
p5 := 155.2;  p6 := 242.5;

# Survival and transition probabilities
p7 := 0.7;    p8 := 0.4;    p9 := 0.08;   p10 := 0;
p11 := 0;     p12 := 0;     p13 := 0;     p14 := 0.3;
p15 := 0.5;   p16 := 0.09;  p17 := 0;     p18 := 0;
p19 := 0;     p20 := 0;     p21 := 0.25;  p22 := 0.6;
p23 := 0.1;   p24 := 0;     p25 := 0;     p26 := 0;
p27 := 0;     p28 := 0.2;   p29 := 0.7;   p30 := 0.10;
p31 := 30;    p32 := 0;     p33 := 0;     p34 := 0;
p35 := 0.15;  p36 := 0.8;

# Initial population by age class
x1 := 50; x2 := 40; x3 := 30;
x4 := 20; x5 := 10; x6 := 5;

# Construct Lefkovitch Matrix
L := Matrix(6,6,
[[p1, p2, p3, p4, p5, p6],
 [p7, p8, p9, p10, p11, p12],
 [p13, p14, p15, p16, p17, p18],
 [p19, p20, p21, p22, p23, p24],
 [p25, p26, p27, p28, p29, p30],
 [p31, p32, p33, p34, p35, p36]]);

# Initial Population Vector
xdist0 := Matrix(6,1, [[x1],[x2],[x3],[x4],[x5],[x6]]);
totpop0 := sum(xdist0);

# Output
Initial vector: [50, 40, 30, 20, 10, 5]
Total initial population = 155

Normalized distribution:
[10/31, 8/31, 6/31, 4/31, 2/31, 1/31]

# One-Season Projection
xdist1 := MatrixMatrixMultiply(L, xdist0);
totpop1 := sum(xdist1);
xdist1 / totpop1;

# Output (t = 1)
[6062.50,
 53.40,
 28.80,
 20.50,
 11.50,
 1505.50]

Total = 7682.20

Proportions:
[0.7892, 0.0069, 0.0037, 0.0026, 0.0015, 0.1959]

# Two-Season Projection for Population A
xdist2 := MatrixMatrixMultiply(L, xdist1);
totpop2 := sum(xdist2);
xdist2 / totpop2;

# Output (t = 2)
[370293.62,
 4267.41,
 32.27,
 20.65,
 162.70,
 183081.12]

Total Population A = 557,857.77

Final proportions:
[0.6638, 0.0076, 0.00006, 0.00003, 0.00029, 0.3282]

# Stability Analysis
A, B := Eigenvectors(L);
A;

# Eigenvalues
[-146.60,
 147.47,   ← dominant λ
 0.7938,
 0.2568,
 0.6287,
 0.4560]

Interpretation: λ = 147.47 indicates long-term population growth.

# Parameters of Population B
p2 := 28.8;  p3 := 115.2;  p4 := 259.2;
p5 := 460.8; p6 := 720;

# Two-Season Projection for Population B
# Using same structure with updated fecundity
# Output (t = 2)

[1.099e6,
 12623.66,
 32.27,
 20.65,
 162.70,
 541206.12]

Total Population B = 1,653,473.88

Final proportions:
[0.6649, 0.0076, 0.00002, 0.00001, 0.00009, 0.3273]
```
