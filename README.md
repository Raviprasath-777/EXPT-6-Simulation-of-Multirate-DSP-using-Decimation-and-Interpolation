# EXPT-6-Simulation-of-Multirate-DSP-using-Decimation-and-Interpolation

# AIM: 

# To perform and verify Multirate-DSP-using-Decimation-and-Interpolation.

# APPARATUS REQUIRED: 
PC installed with SCILAB. 

# PROGRAM: 
```
clc;
clear;
close;

n = 0:1:50;
f = 0.05;
x = sin(2 * %pi * f * n);

M = 3;
y = x(1:M:$);

n_dec = 0:1:(length(y)-1);

figure;
subplot(2, 1, 1);
plot2d3(n, x);
h1 = gce();
h1.children(1).thickness = 3;
plot(n, x, 'ro');
h2 = gce();
h2.children(1).thickness = 2;
h2.children(1).mark_size = 3;
xtitle('Original Signal', 'n', 'x(n)');
xgrid(1);

subplot(2, 1, 2);
plot2d3(n_dec, y);
h3 = gce();
h3.children(1).thickness = 3;
plot(n_dec, y, 'ro');
h4 = gce();
h4.children(1).thickness = 2;
h4.children(1).mark_size = 3;
xtitle('Decimated Signal', 'n', 'y(n)');
xgrid(1);
```

# OUTPUT: 
<img width="1600" height="744" alt="image" src="https://github.com/user-attachments/assets/1480a26c-34b8-49eb-82ca-ff9639a45e37" />


# RESULT: 
Thus the Multirate-DSP-using-Decimation-and-Interpolation using python was performed and verified.
