# WikiPlay
Experimenting on Wikipedia dump


1. Extracting articles from compressed dump:

  $ python make_wiki_corpus enwiki-latest-pages-articles.xml.bz2 wiki_en.txt
  
2. Wikipedia dump file then resulted in a very large corpus file. Given its enormous size, you may have dificulty reading the full file into memory at one time.

The script check_wiki_corpus, then, starts by reading 50 lines -- which equates to 50 full articles -- from the text file and outputting them to the terminal, after which you can press a key to output another 50, or type 'STOP' to quit.Reading file chunks

  $ python check_wiki_corpus.py wiki_en.txt
