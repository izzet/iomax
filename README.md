# IOMax: Maximizing Out-of-Core I/O Analysis Performance on HPC Systems

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8393987.svg)](https://doi.org/10.5281/zenodo.8393987)

## Abstract

I/O analysis is an essential task for improving the performance of scientific applications on high-performance computing (HPC) systems. However, current analysis tools, which often use data drilling techniques (iterative exploration for deeper insights), treat every query independently and do not optimize column data for data-slicing (extracting specific data subsets), resulting in subpar querying performance. In this paper, we designed IOMax, a tool for efficient data drilling analysis on large-scale I/O traces. IOMax utilizes a novel query optimization technique to improve the query performance by 8.6x while reducing the memory footprint required for analysis by 11x. Additionally, it employs data transformation techniques to improve data-slicing performance by up to 11.4x. In conclusion, IOMax optimizes I/O analysis for scientific workflows on the Lassen supercomputer, resulting in up to 7x improvement.

## Run Evaluations

Create a Python environment via preferred tool. For example:

```bash
python3 -m venv myenv
source myenv/bin/activate
```

Install Python dependencies:

```bash
pip3 install -r requirements.txt
```

Run Jupyter via preferred tool. For example:

```bash
jupyter notebook 
jupyter lab
```

Open `evaluations.ipynb` and follow the steps.

> [!NOTE]
> We run the experiments on the Lassen supercomputer at Lawrence Livermore National Laboratory (LLNL). A 23-petaflop IBM Power9 system consists of 795 nodes connected with a Mellanox 100 Gb/s EDR InfiniBand network, and a 24 PiB IBM Spectrum Scale file system (also known as GPFS). Individual Lassen nodes consist of two IBM POWER9 CPUs (IBM AC922 servers) with 256GB of system memory.

## Acknowledgments

<small>This work was performed under the auspices of the U.S. Department of Energy by Lawrence Livermore National Laboratory under Contract DE-AC52-07NA27344. This material is based upon work supported by the U.S. Department of Energy, Office of Science, Office of Advanced Scientific Computing Research under the DOE Early Career Research Program (LLNL-CONF-852637). Also, the material is based upon work supported by the National Science Foundation under Grant no. NSF OAC-2104013,  OCI-1835764, and CSR-1814872.</small>