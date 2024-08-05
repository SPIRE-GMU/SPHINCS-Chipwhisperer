# SPHINCS-Chipwhisperer

This repository implements Faulty Injection attacks on SPHINCS+, and comes up with a countermeasure by masing the address using a counter.  

***Structure***

crypto: SPHINCS+ source codes

simpleserial-sphincsplus: attack template

***Setup***

1. Install Chipwhisperer: https://chipwhisperer.readthedocs.io/en/latest/

2. Copy (crypto & simpleserial-plus) into chipwhisperer/hardware/victims/firmware installaion folder

3. Open jupyter-notebook and follow the kernel sphincs.ipython

   **Note** There may be direction issues when compiling and programming the simpleserial-sphincs. Please feel free to change.

