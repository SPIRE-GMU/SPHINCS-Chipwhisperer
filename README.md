# SPHINCS-Chipwhisperer

This repository implements Faulty Injection attacks on SPHINCS+, and comes up with a countermeasure by masing the address using a counter.  You may follow the exp_script/sphincs.ipython and learn how to send commands, how to send glitches, and finally how to implement FA to SPHINCS+. 

***Structure***

  1.  crypto: SPHINCS+ source codes (It runs in the victim device)

  2.  simpleserial-sphincsplus: attack template (Chipwhisperer board sends glitches and collects values. )

  3.  sphincs.ipython: A script where the host communicates with Chipwhisperer board. We provide a .ipython script for a step-by-step debug hoping it offers a better  understanding to the reader.

  4. draw_3d_result.ipython: Once you collect results using the attack script, you can draw a 3-D figure telling which glitch succeeds.

***Setup***

1. Install Chipwhisperer: https://chipwhisperer.readthedocs.io/en/latest/

2. Copy (crypto & simpleserial-plus) into chipwhisperer/hardware/victims/firmware installation folder. (Replace the Makefile.crypto)

3. Open jupyter-notebook and follow the kernel sphincs.ipython

   **Note** There may be direction issues when compiling and programming the simpleserial-sphincs. Please feel free to change.

***Reference***

