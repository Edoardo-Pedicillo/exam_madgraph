# Exercise 1.6

Generate and output the folder for $pp \rightarrow t\bar{t}$ at NLO with `MG5aMC`. Using
that directory:

(a) Calculate the cross section at LO and LO+PS (using `Pythia8` as
shower).
Hint: use the analyses `analysis_HwU_pp_ttx_v2` and `py8an_HwU_pp_ttx_v2`
for the two runs, respectively, and note that they have to be set
inside different cards.
What is the K-factor? Can you explain the differences between
the LO and LO+PS distributions?

(b) Calculate $\sigma_\text{NLO}(pp \rightarrow t \bar{t})$ with `MG5aMC`. What is the K-factor?
Comment and explain the differences between the LO and NLO distributions.

## Solution

### NLO
```
--------------------------------------------------------------
  Final results and run summary:
  Process  p p > t t~ [QCD]
  Run at p-p collider (6500.0 + 6500.0 GeV)
  Total cross section: 6.819e+02 +- 3.6e+00 pb
--------------------------------------------------------------
  Scale variation (computed from histogram information):
      Dynamical_scale_choice -1 (envelope of 9 values):
          6.815e+02 pb  +9.8% -11.8%
--------------------------------------------------------------
```

### LO+PS
```
--------------------------------------------------------------
  Final results and run summary:
  Process  p p > t t~ [QCD]
  Run at p-p collider (6500.0 + 6500.0 GeV)
  Total cross section: 4.559e+02 +- 2.0e+00 pb
--------------------------------------------------------------
  Scale variation (computed from histogram information):
      Dynamical_scale_choice -1 (envelope of 9 values):
          4.559e+02 pb  +29.7% -22.2%
--------------------------------------------------------------
```


### LO 
```
--------------------------------------------------------------
  Final results and run summary:
  Process  p p > t t~ [QCD]
  Run at p-p collider (6500.0 + 6500.0 GeV)
  Total cross section: 4.569e+02 +- 1.9e+00 pb
--------------------------------------------------------------
  Scale variation (computed from histogram information):
      Dynamical_scale_choice -1 (envelope of 9 values):
          4.569e+02 pb  +29.7% -22.3%
--------------------------------------------------------------
```

The K factor is the ratio between two cross sections:
    - for LO+PS and LO is 0.997+-0.006
    - for NLO and LO is 1.49+-0.01.

Regarding the LO and LO+PS distributions stored in `lo.pdf` and `lo_ps.pdf`, there are no differences, even though I am 
expecting more particles are emitted in the second case, I suspect the script is generating wrong results.
The NLO calculation leads to a non-trivial transverse momentum distribution for the 
$t \bar{t}$ pair compared to the LO one.

