# Exercise 1.4

Calculate $\sigma(e^+e^- \rightarrow q \bar{q})$ \@ NLO with $\texttt{MG5aMC}$. What is the $K$-factor?

## Solution

To evaluate the cross sections, execute `ex1_4.mg5` through the command:
```
mg5_aMC ex1_4.mg5
```
The cross sections of the process `e+ e- > q q~` are the following:

### LO
```
--------------------------------------------------------------
  Final results and run summary:
  Process e+ e- > q q~ [QCD]
  Run at l-l collider (500.0 + 500.0 GeV)
  Total cross section: 5.334e-01 +- 3.2e-03 pb
--------------------------------------------------------------
  Scale variation (computed from histogram information):
      Dynamical_scale_choice -1 (envelope of 9 values):
          5.334e-01 pb  +0.0% -0.0%
--------------------------------------------------------------
```

### NLO

```
--------------------------------------------------------------
  Final results and run summary:
  Process e+ e- > q q~ [QCD]
  Run at l-l collider (500.0 + 500.0 GeV)
  Total cross section: 5.476e-01 +- 1.9e-03 pb
--------------------------------------------------------------
  Scale variation (computed from histogram information):
      Dynamical_scale_choice -1 (envelope of 9 values):
          5.472e-01 pb  +0.2% -0.2%
--------------------------------------------------------------
```
The K-factor is the ratio of NLO and LO, i.e., 1.026+-0.007. 
