This is a Python implementation of K-Means clustering algorithm using the Map Reduce paradigm.
It is customized for processing a thunders dataset, extracted from [STARNET (Sferics Timing And Ranging NETwork)](http://www.zeus.iag.usp.br)
Under **src/** folder are the mapper and reducer scripts that can be run on a Hadoop environment. There is also a script to run the Hadoop job on Amazon Elastic Map Reduce (run_kmeans_emr.py).
Under **data/** folder is a sample of the thunders that "falled" on February 28, 2014.
Under **results/** folder are CSV datasets contained all thunders of that date in a single file and the resulting clusters (for k=10 and k=50).

In the picture bellow are presented the thunders distribution map and a heat map to show concentration.
![Mapas da distribuição de raios e mapa de calor](http://workingsweng.com.br/wp-content/uploads/2014/04/Map_Points_unified.png) 

In these mapas, you can see the generated cluster distribution (for k=10 and k=50) against the heat map, showing that K-Means algorithm worked as expected.
![Mapas com os clusters gerados (k=10 e k=50)](http://workingsweng.com.br/wp-content/uploads/2014/04/Map_Points_unified2.png) 

A detailed description of the problem and this implementation is available on http://workingsweng.com.br/2014/04/clusterizando-raios-com-hadoop-e-k-means-em-map-reduce/
