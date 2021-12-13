# Men Are Elected, Women Are Married: Events Gender Bias on Wikipedia

Code and Data for our ACL paper "[**Men Are Elected, Women Are Married: Events Gender Bias on Wikipedia**](https://vnpeng.net/bibliography/sun2021men)"

Please cite us if you find any of these content useful.

```
@inproceedings{sun2021men,
  title = {Men Are Elected, Women Are Married: Events Gender Bias on Wikipedia},
  author = {Sun, Jiao and Peng, Nanyun},
  booktitle = {Proceedings of the Conference of the 59th Annual Meeting of the Association for Computational Linguistics (ACL)},
  year = {2021}
}
```



## Dependencies

When using Python>=3.7.6, ensure to download the follwing packages into your python developent environment either with pip3 or conda (depending on the development tools you use)
- pandas
- spacy
- seaborn
- matplotlib
- gensim



## Code

1. **Analysis Pipeline**. 
  - The authors original code and results are duplicated in `original.ipynb`. These contain the key steps used in the paper - including acquire and populate templates by name swaping, odds ratio calculation, replicate figures.
  -  The results from our reproduction are in `reproduce.ipynb`.
  -  Finally, the code and results for the ablation study are in the file `ablate.ipynb`.
3. **WEAT calculation**. The code for replicating our WEAT calculation is under `WEAT.py`, please see how to use in `./weat.sh` to replicate the result. You can simply change the list of dictionary in `artists.json` and use our script to measure the associated gender bias of any two lists of attributes. 



## Data & Download

   ### Complete Corpus 

1. Please find all collected data under [here](https://drive.google.com/drive/folders/1JaX0uX7Joriaz6K5QcuLdnWA1GGBX18J?usp=sharing) where you can access all sections that we collected, statistics in Appendix Table 6, and put them under `data/raw-data`

   ### Analysis Necessarities 

2. The data we use fo analyzing the <em>career</em> and <em>Personal Life</em> sections are under `data/ee-fm`

3. The intermediate results which contain extracted events for each section are under `data/ee-model`

   ### WEAT score embeddings

4. Please download the embeddings under [here](https://drive.google.com/drive/folders/1JaX0uX7Joriaz6K5QcuLdnWA1GGBX18J?usp=sharing) and put them under `WEAT/embeddings/` folder







 

