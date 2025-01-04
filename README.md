# rna_seq_snakemake

Download the SRA files:

70-15 SRR081554
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/SRR081/SRR081554/SRR081554_2.fastq.gz
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/SRR081/SRR081554/SRR081554_1.fastq.gz

70-15 ERR6065780
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/ERR606/000/ERR6065780/ERR6065780_2.fastq.gz
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/ERR606/000/ERR6065780/ERR6065780_1.fastq.gz

Guy11 ERR6065780
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/ERR606/000/ERR6065780/ERR6065780_2.fastq.gz
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/ERR606/000/ERR6065780/ERR6065780_1.fastq.gz

Guy11 ERR3890143
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/ERR389/003/ERR3890143/ERR3890143_1.fastq.gz
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/ERR389/003/ERR3890143/ERR3890143_2.fastq.gz

B157 SRR1747212
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/SRR174/002/SRR1747212/SRR1747212_2.fastq.gz
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/SRR174/002/SRR1747212/SRR1747212_1.fastq.gz

B157 SRR17410088 
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/SRR174/088/SRR17410088/SRR17410088_2.fastq.gz
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/SRR174/088/SRR17410088/SRR17410088_1.fastq.gz

P131 SRR31346807
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/SRR313/007/SRR31346807/SRR31346807_1.fastq.gz
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/SRR313/007/SRR31346807/SRR31346807_2.fastq.gz

P131 SRR31346810
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/SRR313/010/SRR31346810/SRR31346810_1.fastq.gz
wget -nc ftp://ftp.sra.ebi.ac.uk/vol1/fastq/SRR313/010/SRR31346810/SRR31346810_2.fastq.gz


mamba create -n rna-seq python=3.9
mamba activate rna-seq 
mamba install fastqc -c bioconda
fastqc - *fastq.gz
mamba install -c bioconda trimmomatic

