# `pytcspc`: analysis of time-correlated single photon counting (TCSPC) data

This python library can be used for analyzing time-domain fluorescence lifetime imaging microscopy (FLIM) data and fluorescence correlation spectroscopy (FCS) data collected with TCSPC hardware.

## Installing
Please see [`INSTALLATION.md`](https://github.com/easunarunachalam/pytcspc/blob/master/INSTALLATION.md).

## Functions

### FLIM
- read Becker &amp; Hickl .sdt files (based on [`sdtfile`](https://github.com/cgohlke/sdtfile)) into user-friendly `xarray.DataArray`s suitable for further analysis
- produce intensity and lifetime images
- fit decay curves to multiexponential models using least-squares or Gibbs sampling approaches

### FCS
- read Becker &amp; Hickl .spc files into user-friendly `xarray.DataArray`s suitable for further analysis
- generate FLIM and intensity images and "videos"
- generate kymographs for line-scanning FCS
- calculate correlation functions (based on [`multipletau`](https://github.com/FCS-analysis/multipletau))

## examples
- `FCS`: fit FCS data for diffusion of Alexa Fluor 488
- `fit_oneexp`: fit decay curve for a solution of FAD
- `fit_from_image`: fit decay curve for NAD(P)H in yeast
- `Gibbssampling`: fit a polyexp model using least-squares regression and a biexponential model using Gibbs sampling

## Contributing
Please see [`CONTRIBUTING.md`](https://github.com/easunarunachalam/pytcspc/blob/master/CONTRIBUTING.md).
