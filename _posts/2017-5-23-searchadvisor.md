---
layout: post
title: Search your advisor application!
---

Designed and developed a search based framework using Apache Solr to index the professors based on their research areas. Crawled professor information from top 30 US universities using Python. Integrated a web interface using PHP, Javascript, HTML.



![_config.yml]({{ site.baseurl }}/images/searchyouradvisor.png)

* To get the required data from the required websites we can use multiple ways to get it by making the crawler. A web crawler also known as spider, is a program or automated script which browses the World Wide Web in an automated manner. The process is called Web crawling or spidering.
Web crawlers are mainly used to create a copy of all the visited pages for later processing by a search engine, that will index the downloaded pages to provide fast searches.
There are multiple ways to crawl the websites for the faculty by using different programming languages like Java and PHP. The data taken from crawling is also produced in multiple formats XML and CSV. But, in this project crawling is done using Beautifulsoup library in Python and then storing all the data that is achieved during crawling in JSON formats as shown in fig.

* JSON files are fed to the Solr, which is an open source, stand alone, fault tolerant and highly reliable Apache Lucene project. Solr has in built algorithms that helps us to do the search and rank them based on the relevance. This also provides us the URL where we can modify the q term and perform the search based on the user interest.

![_config.yml]({{ site.baseurl }}/images/advisorschema.PNG)

*Source code located at* [this repository](https://github.com/vdsc/Advisor-recommendation)

* a User interface is designed so that the user query is used to get the search results from Solr and display them on the page. This is achieved by using PHP to interact with the User Interface and the Solr. 
