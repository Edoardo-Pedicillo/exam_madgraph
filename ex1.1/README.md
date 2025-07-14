# Exercise 1.1

Calculate the partial widths of the Z and W bosons and the t quark and
compare with the analytic formulas you find in preferred QFT book.

## Solution

The width of the different particles are obtained launching the following commands:

```
mg5_aMC ex1_1_{t,w,z}.mg5
```

The outputs are the following:

- t-quark
    ```
         Width :   1.491 +- 5.537e-05 GeV
    ```
- Z boson
    ```

         Width :   2.442 +- 9.599e-05 GeV
    ```
- W boson
    ```
         Width :   2.048 +- 7.043e-05 GeV
    ```

The results are close to the measured ones:

- `W` and `Z`: [PDG _gauge and higgs_ bosons section](https://pdg.lbl.gov/2025/tables/rpp2025-sum-gauge-higgs-bosons.pdf)
- `t`: [PDG _quarks_ section](https://pdg.lbl.gov/2025/tables/rpp2025-sum-quarks.pdf)
