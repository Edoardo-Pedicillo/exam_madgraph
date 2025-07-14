# Exercise 1.5

Calculate $\sigma(pp \rightarrow e^+ e^-)$ \@ NLO with $\texttt{MG5aMC}$. What is the $K$-factor?
Using the analysis `analysis_HwU_pp_lplm`, comment and explain the
differences between the LO and NLO distributions.

## Solution
The cross sections are evaluated running the following command:

```
mg5_aMC ex1_5.mg5
```

### NLO
```
--------------------------------------------------------------
  Summary:
  Process p p > e+ e- [QCD]
  Run at p-p collider (6500.0 + 6500.0 GeV)
  Number of events generated: 10000
  Total cross section: 2.097e+03 +- 4.6e+00 pb
--------------------------------------------------------------
  Scale variation (computed from LHE events):
      Dynamical_scale_choice -1 (envelope of 9 values):
          2.091e+03 pb  +5.7% -11.2%
--------------------------------------------------------------
```

### LO 
```

--------------------------------------------------------------
  Summary:
  Process p p > e+ e- [QCD]
  Run at p-p collider (6500.0 + 6500.0 GeV)
  Number of events generated: 10000
  Total cross section: 2.094e+03 +- 4.7e+00 pb
--------------------------------------------------------------
  Scale variation (computed from LHE events):
      Dynamical_scale_choice -1 (envelope of 9 values):
          2.082e+03 pb  +6.3% -11.7%
--------------------------------------------------------------

```
The K factor between NLO and LO is 1.001+-0.003
While generating the results I was getting an error reported in `mcatnlo.log` and
I was not able to generate the histogram.
