
# Basic MATLAB Operations

by Your Name on March 7th, 2024

## Mathematical Expressions
-  Basic Arithmetic Operaions: $-4+\frac{7\times (2-5f)}{\pi }$ 
```matlab
a = -4 + (7 * (2-5)) / pi 
```

```matlabTextOutput
a = -10.6845
```

-  Powers and Squreroots: $2^3 -\sqrt{25}+e^3$ 
```matlab
b = 2^3 - sqrt(25 + exp(3))
```

```matlabTextOutput
b = 1.2854
```

-  Complex Numbers: $(2+3i)(1-2i)^2$ 
```matlab
c = (2 + 3i) * (1-2i)^2
```

```matlabTextOutput
c = 6.0000 -17.0000i
```
## Generating Arrays, aka Vectors
-  Zeros and Ones 
```matlab
z = zeros(1,3)
```

```matlabTextOutput
z = 1x3
     0     0     0

```

```matlab
k = ones(4)
```

```matlabTextOutput
k = 4x4
     1     1     1     1
     1     1     1     1
     1     1     1     1
     1     1     1     1

```

```matlab
w = 9 * ones(2,4)
```

```matlabTextOutput
w = 2x4
     9     9     9     9
     9     9     9     9

```

-  Evenly Spaced Numbers 
```matlab
s = 10:2:20
```

```matlabTextOutput
s = 1x6
    10    12    14    16    18    20

```

```matlab
sl = length(s)
```

```matlabTextOutput
sl = 6
```

```matlab
m = 10:-2:2
```

```matlabTextOutput
m = 1x5
    10     8     6     4     2

```

```matlab
n = linspace(1, 2, 11)
```

```matlabTextOutput
n = 1x11
1.0000    1.1000    1.2000    1.3000    1.4000    1.5000    1.6000    1.7000    1.8000    1.9000    2.0000

```
## Matrix Operations
-  Operations on Matrix with a Scalar 
```matlab
M = magic(3)
```

```matlabTextOutput
M = 3x3
     8     1     6
     3     5     7
     4     9     2

```

```matlab
M1 = M - 1
```

```matlabTextOutput
M1 = 3x3
     7     0     5
     2     4     6
     3     8     1

```

```matlab
M2 = 2*M
```

```matlabTextOutput
M2 = 3x3
    16     2    12
     6    10    14
     8    18     4

```

```matlab
M3 = 1./M
```

```matlabTextOutput
M3 = 3x3
    0.1250    1.0000    0.1667
    0.3333    0.2000    0.1429
    0.2500    0.1111    0.5000

```

-  Operations on Two Matrices 
```matlab
N1 = randi(9, 2, 3)
```

```matlabTextOutput
N1 = 2x3
     1     8     2
     5     9     6

```

```matlab
[r,c] = size(N1)
```

```matlabTextOutput
r = 2
c = 3
```

```matlab
N2 = randi(9, 2, 3)
```

```matlabTextOutput
N2 = 2x3
     5     4     8
     1     2     3

```

```matlab
N3 = N1 + N2
```

```matlabTextOutput
N3 = 2x3
     6    12    10
     6    11     9

```

```matlab
E1 = eye(2)+1
```

```matlabTextOutput
E1 = 2x2
     2     1
     1     2

```

```matlab
E2 = [1 1; 1 0]
```

```matlabTextOutput
E2 = 2x2
     1     1
     1     0

```

```matlab
E3 = E1 * E2
```

```matlabTextOutput
E3 = 2x2
     3     2
     3     1

```
## Part of Matrices
```matlab
R = magic(4)
```

```matlabTextOutput
R = 4x4
    16     2     3    13
     5    11    10     8
     9     7     6    12
     4    14    15     1

```

```matlab
r1 = R(2, :)
```

```matlabTextOutput
r1 = 1x4
     5    11    10     8

```

```matlab
r2 = R(2:3, 2:3)
```

```matlabTextOutput
r2 = 2x2
    11    10
     7     6

```
## Basic Statistics
```matlab
k = round(10*sin(0:10))
```

```matlabTextOutput
k = 1x11
     0     8     9     1    -8   -10    -3     7    10     4    -5

```

```matlab
[min(k), max(k), mean(k), median(k), var(k)]
```

```matlabTextOutput
ans = 1x5
  -10.0000   10.0000    1.1818    1.0000   49.3636

```

```matlab
k1 = sort(k)
```

```matlabTextOutput
k1 = 1x11
   -10    -8    -5    -3     0     1     4     7     8     9    10

```
