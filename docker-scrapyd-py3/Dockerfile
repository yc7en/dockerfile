#
# latest scrapyd 1.2.0 add python3 support
# based on offical python:3.6.1
# scrapyd doc: http://scrapyd.readthedocs.io/en/latest/
# add some useful tools
#

FROM python:3.6.1

MAINTAINER yc7en

RUN	set -ex \
	&& pip install scrapy==1.3.3 \
				   scrapyd==1.2.0 \
				   scrapyd-client \
	&& rm -rf /tmp/*   

COPY ./scrapyd.conf /etc/scrapyd/

VOLUME /etc/scrapyd/ /var/lib/scrapyd/

EXPOSE 6800

CMD scrapyd