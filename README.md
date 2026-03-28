# Modular Bootstap

Version 1.0.0

Corresponding author:  Jesse Thaler <jthaler@mit.edu>

Additional contributions:  Nathan Benjamin <nathanbe@usc.edu>, Liam Fitzpatrick <fitzpatr@bu.edu>, Wei Li <weili17@bu.edu>

## Context ##

This Mathematica code regenerates all of the figures and tables from arXiv:2604.xxxxx, related to solving the numerical modular bootstrap using machine-learning-style optimization.

## Known Issues ##

- Speed:  While the optimization runs have been stored, additional post-processing has not, so it can be very slow to recompute everything in the notebook.
- Memory management:  There are cases where extraneous information is being cached, which causes excess memory usage when doing long optimization runs.
- Derivative computations:  There are cases where derivatives with respect to parameters are computed after substituting numerical values from the training data, which is highly inefficient.
- Copied/pasted code:  There are certain parts of the code, especially related to executing the survey results, with copy/pasted elements that hadn't been turned into cleaner functions.
- No AI assistance:  At the time this code was originally written, agentic AI systems were making too many mistakes to be useful for this project, so all of the code is human written.  Future versions will be streamlined and improved as the capabilities of agents improve.

