# Interactive Sketchmap Visualizer

The code to generate Interactive Sketchmap visualizer using bokeh. 
To see an demo version try : https://sketchmap.herokuapp.com/
To know about sketchmap go to http:/sketchmap.org/



# Usage

 bokeh serve example-app --show --args -u 1:2:3 -ps 10 

To use your own data you have to do the following 
cp -r example-app  <your-app>
cp <SMAP-DATA-FILE> <your-app>/data/COLVAR
rm -f <your-app>/static/xyz/*
cp <your-xyz-files> <your-app>/static/xyz/

<SMAP-DATA-FILE> format
Column-Name-1 Coulumn-Name-2  ... ... ...
data11         data12         ... ... ...
  :              : 
  :              :
  :              :


<your-xyz-files> need to follow the name convention: set.0000.xyz set.0001.xyz .....

# Dependencies

argparse

tornado==4.4.3

numpy

bokeh==0.12.5

pandas
