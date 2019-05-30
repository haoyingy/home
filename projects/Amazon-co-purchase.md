---
layout: post
title: 'Amazon Co-Purchase Social Network'
---

**Project Overview**
* This project is about Amazon’s co-purchase network with over 1 million products sales record and other features
* The goal is to analyze co-purchase data to build a social network among products and identify key metrics for sales 
* We analyzed relationship between products by metrics such as closeness and betweenness via NetworkX in Python, and iGraph via R
* Visualized products relationship with a net of nodes and edges via Python, showing relationships among products 
* Identified influential metrics related to sales rank by applying Poisson Regression via GLM in R
* Discovered relationships among over 200,000 book products; found 8 significant influential factors for book sale
<br><br>

![](https://raw.githubusercontent.com/haoyingy/Home/gh-pages/assets/img/projects/proj-3/network.png)

The graph demonstrates 904 vertices. These 904 vertices are the book ids that connected to the book whose id = 33, directly and indirectly. <br>
Size of the vertices represents the number of vertices that connected to a vertice, the bigger of the vertice, the more vertices link to it.<br> 
The distance between each vertice represents how strong the vertices connect to each other, the longer the ties, the weaker the relationship. <br>
Therefore, some vertices look like clusters in the middle with short edges, which means these books have strong connections. Some vertices are nodes on the edges, which means weaker connections. 
<br><br>
There are two data files: “products.csv” and “copurchase.csv”. “products.csv” contains the information about the products. “copurchase.csv” contains the co-purchase information (i.e., if people bought one product, then they also co-purchased the other). link to details on Rpubs [here](http://rpubs.com/Ericyang95/481280) Or more details on [github]('https://github.com/haoyingyang/SN')


