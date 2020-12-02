### Convert bedgraph to bigwig
```bash
sort -k1,1 -k2,2n unsorted.bedGraph > sorted.bedGraph
rm *unsorted.* # remove the original bedgraph files
# convert bg to bw
bedGraphToBigWig in.bedGraph chrom.sizes out.bw
rm *bedGraph # only leaves bigwig files
```
## process all files in a directory
```bash
for f in ./*bdg
do
base=$(basename $f | sed 's/.bdg//g')
echo "base: $base"

grep 'Pp' $f > Pp_only/$base.bg
sort -k1,1 -k2,2n Pp_only/$base.bg > Pp_only/$base.sorted.bedGraph
rm Pp_only/$base.bg
bedGraphToBigWig Pp_only/$base.sorted.bedGraph chro_size.txt Pp_only/$base.bw
done
```
