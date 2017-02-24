### VirtualTumorEvolution
A Python script to simulate 3D tumor growth and multi-region sequencing data 
via an agent-based model. Deme subdivision is assumed in order to model cell
mixing and spatial contraint
* Spatial model: peripheral growth

Author
---
* Zheng Hu in Curtis lab@Stanford
* Release Date: 2/23/2017


Requirements
---
Python packages: numpy,sys,math,random,collections,sets

Usage
---

* Simulation of a typical tumor (~10^9 cells) is computationally costly.  We suggest to run this script on HPC cluster. 
* The memory cost is also large, e.g. it costs about ~40G when the final_tumor_size = 10^9 and mut_rate = 0.6.

To run the script

	$ python 3DTumorSimul_MultiRegionSeq.py deme_size mut_rate adv_rate s_coef repl
	e.g., python 3DTumorSimul_MultiRegionSeq.py 5000 0.6 0.00001 0.1 0
