# EnhancerWorkflow -  A workflow to screen enhancers using cis-regulatory elements (CREs)
## Description
A workflow for screening / selecting gene-associated enhancers based on cis-regulatory elements (CREs) and comparative genomics
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
TODO

### Step 2 - Analyse H3K4me1 histone marks to screen for TBX5 enhancers
TODO

### Step 3 - Use Hi-C dataset to further filter TBX5 enhancers from step 2
TODO

### Step 4 - Use comparative genomics to further filter TBX5 enhancers from step 3
TODO

### Step 5 - Visualise TBX5 enhancers idenfitied by this example 
UCSC Genome Browser custom track: http://genome.ucsc.edu/cgi-bin/hgTracks?db=mm9&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr15%3A103004082%2D103088558&hgsid=1134659145_DO3gHeFLzuoFSeD6fYgl2L4SMdFT
![UCSC-Screenshot1](https://github.com/Ramialison-Lab/CardiacNetworkComponentPredictor/raw/main/CardiacNetworkComponentPredictor/images/UCSC-Screenshot1.png)

