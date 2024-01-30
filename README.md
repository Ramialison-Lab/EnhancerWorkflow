# EnhancerWorkflow -  A workflow to screen enhancers using cis-regulatory elements (CREs)
## Description
A workflow for screening / selecting gene-associated enhancers based on cis-regulatory elements (CREs) and comparative genomics.

Manuscript: Jooa Kwon, Hieu T. Nim*, Mirana Ramialison<sup>*</sup>. "EnhancerWorkflow: A web-based workflow to select enhancers for a specific gene-of-interest". (<sup>\*</sup>: corresponding authors)

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
Datasets used in this case study:
![Dataset-Screenshot1](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/Dataset-Screenshot1.png)

VISTAheart (Dickel et al. 2016) data: http://genome.ucsc.edu/cgi-bin/hgTracks?db=mm9&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr15%3A103004082%2D103088558&hgsid=1134659145_DO3gHeFLzuoFSeD6fYgl2L4SMdFT
![UCSC-VISTAheart](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/UCSC-VISTAheart.png)

### Step 2 - Analyse H3K4me1 histone marks to screen for TBX5 enhancers
UCSC Genome Browser custom track: https://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr12%3A113764994%2D114838326&hgsid=1173251107_I55zANRkFa6ma80YxOdLIh2Q3Rxt
![UCSC-Screenshot-Step2](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/UCSC-Screenshot-Step2.png)

### Step 3 - Use Hi-C dataset to further filter TBX5 enhancers from step 2
Hi-C dataset links: https://data.4dnucleome.org/experiments-hi-c/4DNEXCUGCHE3/ and https://data.4dnucleome.org/experiments-hi-c/4DNEXIKZZCZH/
![Hi-C-Screenshot1](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/Hi-C-Screenshot1.png)

### Step 4 - Use comparative genomics to further filter TBX5 enhancers from step 3
UCSC Genome Browser custom track: https://genome.ucsc.edu/cgi-bin/hgTracks?db=mm10&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr5%3A119318425%2D120439424&hgsid=1175114717_4p3oYaBAmnkej8yP6JdfD5R8qadB
![UCSC-Screenshot-Step4](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/UCSC-Screenshot-Step4.png)

### Step 5 - Visualise TBX5 enhancers idenfitied by this example 
UCSC Genome Browser custom track: https://genome.ucsc.edu/cgi-bin/hgTracks?db=mm10&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr5%3A119685600%2D119686720&hgsid=1175114717_4p3oYaBAmnkej8yP6JdfD5R8qadB
![UCSC-Screenshot-Step5](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/UCSC-Screenshot-Step5.png)

### Step 6 - Comparison of predicted TBX5 enhancers with existing TBX5 enhancers from VISTAheart (Dickel et al. 2016)
Galaxy workflow / history: https://usegalaxy.org/u/jooa/h/unnamed-history


UCSC Genome Browser custom track: https://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr12%3A113472654%2D115289720&hgsid=1175084341_at1KnBAOsdqLgahIMAmSWFvJS8xf
![UCSC-Screenshot-Step6](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/UCSC-Screenshot-Step6.png)

### Step 7 - Comparison of predicted TBX5 enhancers with experimentally validated TBX5 enhancers from Smemo et al. 2012
Galaxy workflow / history: https://usegalaxy.org/u/jooa/h/unnamed-history


UCSC Genome Browser custom track: http://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr12%3A113417361%2D114827360&hgsid=1165588985_7U2GpDLLXnWcAL9FRbMZ8LYiaCFl
![UCSC-Screenshot-Step7](https://github.com/Ramialison-Lab/EnhancerWorkflow/raw/main/images/UCSC-Screenshot-Step7.png)


	