`grep -c 'pattern' <filename>`  count how many lines in the file has a word/pattern. 

'cat -n <filename>'  display line number 

* Transfer files       
`scp /source/file destination/` works well with small files.      
`rsync -a source destination` 

* decompress zip files       
`gunzip file.gz`.   unpack gz file  
`unzip file.zip`.   unpack zip file  
`tar -zvf file.tar.gz`.   unpack tar.gz file   

* compress a folder    
`tar -zcvf myfolder.tar.gz myfolder` zip into tar.gz format 
