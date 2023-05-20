# cdhit_cluster_fetch

Author: Murat Buyukyoruk
Associated lab: Wiedenheft lab

        cdhit_cluster_fetch help:

This script is developed to fetch sequences and generates individual cluster fasta outputs by using the CD-HIT .clstr output to fetch. 

SeqIO package from Bio is required to fetch sequences. Additionally, tqdm is required to provide a progress bar since some multifasta files can contain long and many sequences.
        
Syntax:

        python cdhit_cluster_fetch.py -i demo.fasta -l demo_sub_list.txt -o demo_sub_list.fasta

seq_fetch dependencies:

	Bio module and SeqIO available in this package      refer to https://biopython.org/wiki/Download
	tqdm                                                refer to https://pypi.org/project/tqdm/
	
Input Paramaters (REQUIRED):
----------------------------
	-i/--input		FASTA			Specify a fasta file. FASTA file requires headers starting with accession number. (i.e. >NZ_CP006019 [fullname])

	-l/--list		List			Specify a .clstr file generated by CD-HIT.
	
Basic Options:
--------------
	-h/--help		HELP			Shows this help text and exits the run.

