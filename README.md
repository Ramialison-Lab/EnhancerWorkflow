# EnhancerWorkflow -  A workflow to screen enhancers using cis-regulatory elements (CREs)
## Description
A workflow for screening / selecting gene-associated enhancers based on cis-regulatory elements (CREs) and comparative genomics.

Manuscript: Jooa Kwon, Hieu T. Nim, Mirana Ramialison<sup>*</sup>. "A web-based workflow to select enhancers for a specific gene-of-interest". (<sup>\*</sup>: corresponding author)

## Fork the project
To get the source code, please click the "fork" button in the upper-right and then add this repo as an upstream source:

````
$ git clone <your_fork_of_the_repo> ppds
$ cd ppds
$ REPO=https://github.com/Ramialison-Lab/CardiacNetworkComponentPredictor.git
$ git remote add upstream $REPO
````

To get new content, use 
````
$ git pull upstream master 
````

## An example execution of the pipeline - Heart-relevant TBX5 enhancers
### Step 1 - Gather relevant heart-specific datasets for TBX5
Datasets used in this case study:https://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr12%3A113220660%2D114830659&hgsid=1173251107_I55zANRkFa6ma80YxOdLIh2Q3Rxt
![Dataset-Screenshot1](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/Dataset-Screenshot1.png)

### Step 2 - Analyse H3K4me1 histone marks to screen for TBX5 enhancers
UCSC Genome Browser custom track:https://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr12%3A113220660%2D114830659&hgsid=1173251107_I55zANRkFa6ma80YxOdLIh2Q3Rxt
![UCSC-Screenshot1](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/UCSC-Screenshot1.png)

### Step 3 - Use Hi-C dataset to further filter TBX5 enhancers from step 2
Hi-C dataset link (examples): https://data.4dnucleome.org/higlass-view-configs/6762da2c-87d8-4112-854b-04b73ec3d205/ https://data.4dnucleome.org/higlass-view-configs/6762da2c-87d8-4112-854b-04b73ec3d205/
![Hi-C-Screenshot1](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/Hi-C-Screenshot1.png)

### Step 4 - Use comparative genomics to further filter TBX5 enhancers from step 3
UCSC Genome Browser custom track: https://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr12%3A113730352%2D114803684&hgsid=1173255677_vaqbU8wUDolnobVALZf6tw1zohh9
![UCSC-Screenshot1](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/UCSC-Screenshot1.png)

### Step 5 - Visualise TBX5 enhancers idenfitied by this example 
UCSC Genome Browser custom track: http://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr12%3A113391250%2D114801249&hgsid=1165588985_7U2GpDLLXnWcAL9FRbMZ8LYiaCFl
![UCSC-Screenshot1](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/UCSC-Screenshot1.png)

### Step 6 - Comparison of predicted TBX5 enhancers with existing TBX5 enhancers from VISTAheart (Dickel et al. 2016)
UCSC Genome Browser custom track:http://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr12%3A113903382%2D114542381&hgsid=1165588985_7U2GpDLLXnWcAL9FRbMZ8LYiaCFl
![UCSC-Screenshot1](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/UCSC-Screenshot1.png)

### Step 7 - Comparison of predicted TBX5 enhancers with experimentally validated TBX5 enhancers from Smemo et al. 2012
UCSC Genome Browser custom track:http://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr12%3A113903382%2D114542381&hgsid=1165588985_7U2GpDLLXnWcAL9FRbMZ8LYiaCFl
![UCSC-Screenshot1](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/UCSC-Screenshot1.png)
