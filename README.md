# **De Novo Genome Assembly Pipeline**

## Welcome to your ultimate guide for using ready to go, containerized workflows for analyzing genome data.

> So you have sampled your organism of interest, sequenced the data, and found yourself with a bunch of NGS reads that need to be analyzed. But, you don't really know how to proceed, or, you do know, but you would rather spend your time writing your papers or examining other organisms in the meantime. In both cases, you are in the right place at the right time.

![From Reads to Genome](/de-novo.png)

## **What you will find and what will you need to use it**
> The pipeline for genome assembly analyses is made using [Snakemake](https://snakemake.readthedocs.io/en/stable/index.html) and containerized through [Singularity](https://sylabs.io/guides/3.5/user-guide/) with the help of the [Conda](https://docs.conda.io/en/latest/) package manager. If you are not familiar with any of these tools, don't worry. All you have to know, is that these technologies, give you the opportunity to transfer the workflow on any machine, as long as it works with a linux-based kernel and has Singularity installed. If these apply, you can run the pipeline effortlessly, without worrying about releases and packages that may not be compatible with each other. Conda handles that, and creates environments for the Snakemake workflow to run, without interferring with the system you are hosting it into.

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;![SCS](/scs.png)


#### Please credit accordingly:
> Author: Nellie Angelova, Bioinformatician, Hellenic Centre for Marine Research (HCMR) <br>
> Coordinator/ Supervisor: Tereza Manoussaki, Researcher, Hellenic Centre for Marine Research (HCMR)
