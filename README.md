# BinTaxaAssigner


KrakenHLL outputs kmer frequencies per contig in a bin but user needs to visually compare all the contigs within a bin and decode the most appropiate taxnomic level depends on k-mer frequence. BinTaxaAssigner investigate the quality of a hit at species-level, if a species-level hit fails to meet a certain quality threshold it goes to next taxonomic level up to phylum-level. 

1) Run krakenHLL on a bin fasta file as follow:
   https://github.com/fbreitwieser/krakenhll

2) MAG_TaxaAssigner(krakenHll_output)

3) Use a forloop from source_code to run MAG_TaxaAssigner() for all the bins 

4) MAG_TaxaAssigner() prints out the best taxnomic assignment per bin


#MAG_TaxaAssigner() 
This is a function to assign proper taxon to each metagenome assembled bin using a unique k-mer count (the HyperLogLog) algorithm from KrakenHLL. please read KrakenHLL for more information
 https://github.com/fbreitwieser/krakenhll
