# Data visualizations of the bachelor's degree results in metropolitan France

## Table of contents

<ol id="navigation"> 
<li><a href="https://github.com/ArnaudBru/ProjetBAC/blob/master/README.MD#what-is-this-" t>What is this</a></li> 
<li><a href="https://github.com/ArnaudBru/ProjetBAC/blob/master/README.MD#subjects-context">Subject's context</a></li> 
<li><a href="https://github.com/ArnaudBru/ProjetBAC/blob/master/README.MD#data-sources" >Data Sources</a></li> 
<li><a href="https://github.com/ArnaudBru/ProjetBAC/blob/master/README.MD#the-working-approach" >The working approach</a></li> 
<li><a href="https://github.com/ArnaudBru/ProjetBAC/blob/master/README.MD#the-visualization-tool" >The visualization tool</a></li> 

<li><a href="https://github.com/ArnaudBru/ProjetBAC/blob/master/README.MD#video" >Video</a></li> 
</ol> 

## What is this ?

This is a script created by <b> Arnaud Brugière</b> ( https://github.com/ArnaudBru ), <b>Luca Guéry</b> ( https://github.com/guegzz ) and <b>Aurélien VIRELLO</b> ( https://github.com/AurelienVirello ), using the D3.js library. It allows you to visualize results of the <b> bachelor's degree </b>. A version with 2016 datas is hosted on  https://arnaudbru.github.io.

<figure>
<p align="center"> <img src="/img/Global.png" width=80% />
</figure>
<p align="center"> <i>Overview </i> </p>

## Subject's context
<p align=justify>
As part of the course <b> Interactive Data Visualization </b> supervised by <b>Romain Vuillemot </b> at the Ecole Centrale de Lyon, we have set up an interactive visualization project for the <b>results of the 2016 baccalaureate degree in metropolitan France in general and technological secondary schools</b>.
Our tool was created to obtain an <b>overview of the 2016 results</b>. We have worked to create a <b>global and geographical visualization</b> tool, but also a detailed one, with a <b>visual per branch and per staff of each establishment</b>.
</p>

## Data Sources

<p align=justify>
The results data of resulats used are freely downloadable on the French government's open data portal and are available at the following address: 
</p>
<p align=justify>
<a href="https://www.data.gouv.fr/fr/datasets/indicateurs-de-resultat-des-lycees-denseignement-general-et-technologique/#">https://www.data.gouv.fr/fr/datasets/indicateurs-de-resultat-des-lycees-denseignement-general-et-technologique/#</a>
</p>
<p align=justify>
The data contain various indicators of the success of institutions at the baccalaureate level :
<ul>
  <li> The success rate by sector   </li>
  <li> Staffing by sector  </li>
  <li> The sector (public/private)  </li>
  <li> Name of the secondary schools   </li>
  <li> Geographical position of secondary schools  </li>
</ul>
</p>
<p align=justify>

Geographic data are also available for free download on : 
<a href="https://github.com/gregoiredavid/france-geojson">https://github.com/gregoiredavid/france-geojson</a>

This GitHub gathers different files in the format <a href="http://geojson.org/">GeoJSON</a> representing all or part of the French territory according to different divisions.The display uses a breakdown by department.
 </p>
 
 ## The working approach

Collaborative work divided into four design sheets has allowed us to guide our work to achieve the desired results. You will find more details of our approach in French <a href="https://github.com/ArnaudBru/ProjetBAC/blob/master/PROPOSAL.MD"> Here </a>
<figure>
<p align="center"> <img src="/img/designsheet4.jpg" width=50% />
</figure>
<p align="center"> <i>Design sheet n°4 </i> </p>

 ## The visualization tool

<p align=justify>
Our tool is divided into three parts, <b>a choropleth map</b>, <b>scatter plot</b> and a <b>bar chart</b>. The three views provide three points of view to study the data. The map provides a <b>global geographical view</b>, while the bar chart provides a real vision on the <b>number of pupils in public and private schools</b>, and the scatter plot allows a more detailed approach and a <b>comparison of the schools by departments.</b>
</p>

 ### Choropleth Map
 
<p align=justify><b>The choropleth map </b>allows you to visualize the success rate in France, by choosing one of the parameters  :
</p>
<ul>
  <li>  <b> TFC </b> : Success rate for all sectors combined </li>
  <li> <b> S </b> : Success rate of the scientific sector </li>
  <li> <b> L </b> : Success rate of the literacy sector </li>
  <li> <b> ES </b> : Success rate of the economical sector </li>
</ul>

<p align=justify>By clicking on a department you can actualize the two others visualizations tools on the department datas.</p>
<figure>
<p align="center"> <img src="/img/Carte.png" width=50% />
</figure>
<p align="center"> <i>Choropleth Map</i> </p>

 ### Bar Chart
 
<p align=justify>The<b> bar chart </b>at the top right-hand side of the site makes it possible to compare headcount between private and public establishments, by sector.
</p>
<figure>
<p align="center"> <img src="/img/barchart1.png" width=80% />
</figure>
<p align="center"> <i>Bar chart - Numbre of students</i> </p>

With a simple click on this graph it is possible to <b>show the success rate by sector</b> and compare the results between <b>public and private </b>schools.
Also, a click function on the departments of the map allows you to <b>update the bar chart on the data of the selected department</b>.

<figure>
<p align="center"> <img src="/img/barchart2.png" width=60% />
</figure>
<p align="center"> <i>Bar chart - Success rate</i> </p>

 ### Scatter plot
 
 <p align=justify>The  <b>scatter plot </b> allows a finer approach per high school. Point monitoring allows you to  <b>visualize the high school and its success rate when you have clicked on a department. Otherwise the graph shows national statistic by department. </b>. 
 <figure>
<p align="center"> <img src="/img/scatter.png" width=60% />
</figure>
<p align="center"> <i>Scatter plot</i> </p>
 
  <p align=justify>
 A memory function allows you to store the display of high schools in  <b>5 departments simultaneously </b>.
</p>
<figure>
<p align="center"> <img src="/img/scatter2.png" width=60% />
</figure>
<p align="center"> <i>Scatter plot</i> </p>

 ## Video
 
  <p align=justify>
  You can watch a video presentation of the visualization tool on the Youtube platform by clicking <a href="https://www.youtube.com/watch?v=gIOnshkxGms&feature=youtu.be"> here </a>.
  </p>
<a href="https://www.youtube.com/watch?v=gIOnshkxGms&feature=youtu.be">
<figure>
  <p align="center"> <img src="/img/Capture.PNG" width=80% />
</figure>
</a>

<p align="center"> <i>Youtube Thumbnail</i> </p>
    <p align=justify>
This video presents the possibilities of the tool and some trends and peculiarities of the 2016 results.
</p>
 
