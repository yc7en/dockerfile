scrapyd-py3
==========================

Scrapyd released 1.2.0 on 2017-04-12. Python3 support added in this version. Other features can be found [here](http://scrapyd.readthedocs.io/en/latest/news.html).

The image based on offical python:3.6.1. Package installed:

	- scrapy==1.3.3
	- scrapyd=1.2.0
	- scrapyd-client 


Please use this as base image for your own project.


docker-compose.yml
---------------------------

    version: '2'
    services:
      scrapyd:
        image: yc7en/scrapyd-py3
        ports:
          - "6800:6800"
        volumes:
          - ./scrapyd:/scrapyd
        container_name: scrapyd
        restart: always


Then you can use it like this:

    docker-compose up -d scrapyd





