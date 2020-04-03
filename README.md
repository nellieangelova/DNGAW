# **De Novo Genome Assembly Pipeline**

## Welcome to your ultimate guide for using ready to go, containerized workflows for analyzing genome data.

> So you have sampled your organism of interest, sequenced the data, and found yourself with a bunch of NGS reads that need to be analyzed. But, you don't really know how to proceed, or, you do know, but you would rather spend your time writing your papers or examining other organisms in the meantime. In both cases, you are in the right place at the right time.

![From Reads to Genome](/de-novo.png)

## **What you will find and what will you need to use it**
> The pipeline for genome assembly analyses is made using [Snakemake](https://snakemake.readthedocs.io/en/stable/index.html) and containerized through [Singularity](https://sylabs.io/guides/3.5/user-guide/) with the help of the [Conda](https://docs.conda.io/en/latest/) package manager. If you are not familiar with any of these tools, don't worry. All you have to know, is that these technologies, give you the opportunity to transfer the workflow on any machine, as long as it works with a linux-based kernel and has Singularity installed. If these apply, you can run the pipeline effortlessly, without worrying about releases and packages that may not be compatible with each other. Conda handles that, and creates environments for the Snakemake workflow to run, without interferring with the system you are hosting it into.

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;![SCS](/scs.png)


> The marriaging of these three tools, create the pipelines and deliver them to you in the form of container images.
> Each ready to use pipeline is represented by an image, and can be run in every cluster or environment that supports the resources and 3d parties tools needed. 
>> In order for you to have some impact on the analysis and to also include your preferences in the procedure, the including and careful filling of a configuration file with lots of parameters by the users is mandatory.

<br>

> Thus, in order for you to run your analysis in your organism's or industry's server, all you need is:

1. A server that has Singularity installed
2. The image of the pipeline you wish to use for your analysis
3. The corresponding configuration file along with the image, that lets you define different parameters for the analysis
4. A script that submits the image as a job into the nodes of your claster


## **Breaking down the steps that lead to the analysis**
> Having found the image that correspond to the analysis you need, download it and copy it along with the configuration file in the *home folder* of your cluster account. A simple cp or a scp will do the trick. Once you're done, open the configuration file with *nano* to edit it. The configuration file is probably the most important component for your analysis to work, so take your time and double check all the paths and the parameters needed here. The file is made to work for all the currently available analyses, so your intervention and filling will in fact let the whole system know which image you are going to use and thus the goal of your chosen pipeline, so make sure to fill the right variables in order for your image to be executed properly. Inside the configuration file you will also find some requirements that your raw data should fullfil. If your data or data directories do not follow the standards, please make the appropriate changes before editing the configurations. <br>
> Once done with all that, it's time to let the automated workflow do the rest for you. Follow the standars for running a job on your server's cluster to submit the image:
```
singularity run <image.simg>
```
***
#### Please credit accordingly:
> Author: Nellie Angelova, Bioinformatician, Hellenic Centre for Marine Research (HCMR) <br>
> Coordinator/ Supervisor: Tereza Manoussaki, Researcher, Hellenic Centre for Marine Research (HCMR)
