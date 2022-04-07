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

# new reccomendations for processing 
http://ftp.1000genomes.ebi.ac.uk/vol1/ftp/data_collections/1000G_2504_high_coverage/20190405_NYGC_b38_pipeline_description.pdf

/storage/datasets/Tetrahymena_thermophila/2017-04-17/read_groups.tsv
/storage/datasets/Tetrahymena_thermophila/2017-04-17/scripts/buildrg.R
#this is the correct one that samples read groups from the first 10 rather than the very first as there may be errors in the first 6N tag
/storage/datasets/Tetrahymena_thermophila/analyses/ancestor_ges_v2/scripts/buildrg.R
