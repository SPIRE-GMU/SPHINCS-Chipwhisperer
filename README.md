# SPHINCS-Chipwhisperer

This repository implements Faulty Injection attacks on SPHINCS+, and comes up with a countermeasure by masing the address using a counter.  You may follow the exp_script/sphincs.ipython and learn how to send commands, how to send glitches, and finally how to implement FA to SPHINCS+. 


## Structure

  1.  crypto: SPHINCS+ source codes (It runs in the victim device)

  2.  simpleserial-sphincsplus: attack template (Chipwhisperer board sends glitches and collects values. )

  3.  sphincs.ipython: A script where the host communicates with Chipwhisperer board. We provide a .ipython script for a step-by-step debug hoping it offers a better  understanding to the reader.

  4. draw_3d_result.ipython: Once you collect results using the attack script, you can draw a 3-D figure telling which glitch succeeds.

## Experimental Configuration 

  ***OS***
  
  Ubuntu 2020.04
  
  ***Software***
  
  1. Python 3.11.0 
  2. jupyter-notebook. There is an issue with the latest version, figure it out with:
  
           pip install traitlets==5.9.0

  ***Hardware***
  
  Chipwhisperer-Lite KIT：  CWLITEARM， target device STM32F3/STM32F4, USB-c, wire.
  
## Setup

1. Install Chipwhisperer: https://chipwhisperer.readthedocs.io/en/latest/

2. Copy (crypto & simpleserial-plus) into chipwhisperer/hardware/victims/firmware installation folder. (Replace the Makefile.crypto)

3. Open jupyter-notebook and follow the kernel sphincs.ipython

   **Note** There may be direction issues when compiling and programming the simpleserial-sphincs. Please feel free to change.

## Reference
[1] Jupyter-notebook issue: https://stackoverflow.com/questions/77138600/why-does-not-jupyter-notebook-open

[2] Standard FA reference: https://github.com/AymericGenet/SPHINCSplus-FA

[3] Chipwhisperer documents: https://chipwhisperer.readthedocs.io/en/latest/getting-started.html

[4] Chipwhisperer tutorial: http://wiki.newae.com/Category:Tutorials
