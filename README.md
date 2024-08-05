# SPHINCS-Chipwhisperer

This repository implements Faulty Injection attacks on SPHINCS+, and comes up with a countermeasure by masing the address using a counter.  You may follow the exp_script/sphincs.ipython and learn how to send commands, how to send glitches, and finally how to implement FA to SPHINCS+. 

***Structure***

crypto: SPHINCS+ source codes (It runs in victim device)

simpleserial-sphincsplus: attack template (Chipwhisperer board sends glitches and collects values. )

exp_script: A script where the host communicates with Chipwhisperer board. We provide a .ipython script for a step-by-step debug hoping it offers a better  understanding to the reader.

***Setup***

1. Install Chipwhisperer: https://chipwhisperer.readthedocs.io/en/latest/

2. Copy (crypto & simpleserial-plus) into chipwhisperer/hardware/victims/firmware installaion folder

3. Open jupyter-notebook and follow the kernel sphincs.ipython

   **Note** There may be direction issues when compiling and programming the simpleserial-sphincs. Please feel free to change.

***Reference***

