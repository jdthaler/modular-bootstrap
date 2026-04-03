# Descending into the Modular Bootstap

_Version 1.0.0_

Contact for code questions/issues:
- Jesse Thaler <jthaler@mit.edu>

Co-authors:
- Nathan Benjamin <nathanbe@usc.edu>
- Liam Fitzpatrick <fitzpatr@bu.edu>
- Wei Li <weili17@bu.edu>

Pre-Print:
- [arXiv:2604.01275](https://arxiv.org/abs/2604.01275)

## Context ##

This Mathematica code regenerates all of the figures and tables from arXiv:2604.xxxxx, related to solving the numerical modular bootstrap equations using machine-learning-style optimization.  The main file is `ml_cft.nb`, which reads in existing optimization results from the `runs` folder.  Plots and tables from the paper are in the `plots` folder, while plots used for debugging appear in `tests`.

## Known Issues ##

- **Speed**:  While the main optimization runs have been stored, additional post-processing has not, so it can be very slow to recompute everything in the notebook, especially uncertainty analyses.
- **Memory management**:  There are cases where extraneous information is being cached, which causes excess memory usage when doing long optimization runs.
- **Order of Operations for Derivatives**:  There are cases where derivatives with respect to parameters are computed after substituting numerical values from the training data, which is still correct, but highly inefficient.
- **Copied/pasted code**:  There are certain parts of the code, especially related to executing the survey results, with copy/pasted elements have not yet been converted into functions.
- **No AI assistance**:  At the time this code was originally written, agentic AI systems were making too many mistakes to be useful for this project, so all of the code is human written (for better or worse; mostly worse).  Future versions will be streamlined and improved as the capabilities of agents have improved.
