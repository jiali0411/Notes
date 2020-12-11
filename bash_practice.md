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

* sort gff3 files based on chromosome order and gene coordinates 
`sort -k1,1V -k4,4n -k5,5rn -k3,3r unsort.gff3 > sorted.gff3`
