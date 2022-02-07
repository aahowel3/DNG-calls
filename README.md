#DNG calls (indel calls using GATK+DNG)
#new working folder located in /work/aahowel3/DNG_calls 
#new command for pushing things with PAT now  git push https://TOKENNAME@github.com/aahowel3/DNG-calls.git master
#running a named command from a makefile with unique name: make -f makefile_practice variables 

#datasets: 
Ancestor nonGEs /storage/datasets/Tetrahymena_thermophila/2017-04-17/fastq - labelled SB210E 1 and 2
Ancestor GEs /storage/datasets/Tetrahymena_thermophila/ancestor_ges 
Descendant nonGEs  /storage/datasets/Tetrahymena_thermophila/2017-04-17/fastq labelled MAs
Descendant GEs  /storage/datasets/Tetrahymena_thermophila/2017-04-17/fastq labelled GEs

#preparing data - concatenating lanes and aligning 
