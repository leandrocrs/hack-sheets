```
############################################################ 
#               COMPRESS                                   # 
#              HACK SHEET LV. 1                            # 
############################################################ 
 
# Para compactar 
rar: $ rar nome_do_arquivo.rar arquivo1 arquivo2 
tar: $ tar -cvvf nome_do_arquivo.tar arquivo1 arquivo2 
tar.bz2: $ tar -cvvjf nome_do_arquivo.tar.bz2 arquivo1 arquivo2 
tar.gz: $ tar -cvvzf nome_do_arquivo.tar.gz arquivo1 arquivo2 
zip: $ zip nome_do_arquivo.zip arquivo1 arquivo2 
 
# Para descompactar 
rar: $ unrar x nome_do_arquivo.rar 
tar: $ tar -xvvf nome_do_arquivo.tar 
tar.bz2: $ tar -xvvjf nome_do_arquivo.tar.bz2 
tar.gz: $ tar -xvvf nome_do_arquivo.tar.gz 
zip: $ unzip nome_do_arquivo.zip 
```