```
--------------------------------------------------------------------------------
orthodotter - Plot orthologous genes on an oxford grid.
       -f <file>     : input file, containing orthologous genes, default is stdin
                       species chr-name start end species chr-name start end
       -toPlot <arg> : give the x and y sets and the color separated by double-dots,
                       for example set1:set2:red will plot set1 on x, set2 on y with
                       red points. Could give several -toPlot arguments.
                       To launch the clustering of dots, use extra-option 1=dist,min_nb_genes
                       where dist is the minimal distance (euclidian) between two points and min_nb_genes the minimal
                       number of genes in a cluster to be valid.
       -o <file>     : output file, default is stdout
       -x <int>      : resolution of x axis, default is 600
       -y <int>      : resolution on y axis, default is 600
       -r <int>      : radius of circle representing orthologous genes
       -format       : could be png, gif, jpg, pdf or ps. Default is png.
       -fg           : foreground color, default is black
       -bg           : background color, default is transparent
       -fSize <int>  : fontSize, default is 1
       -filter       : check chromosome names
       -h            : help
--------------------------------------------------------------------------------
orthodotter -f Vigne_Banane.ortho -toPlot Vigne:Banane:black:1=10,5 -x 1200 -y 1200 -bg white -o Vigne_vs_Banane.png > Vigne_vs_Banane.clusters
--------------------------------------------------------------------------------
```
