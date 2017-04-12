#
# py-kms for /myanaloglife/py-kms
# Supports activating Windows 7/8/8.1/2008R2/2012/2012R2 and Office 2010/2013
#

FROM python:2.7.13-alpine

RUN set xe- \
	&& mkdir /app \
	&& cd /app \ 
	&& apk add --no-cache git \
	&& git clone https://github.com/myanaloglife/py-kms.git \
	&& apk del git 

EXPOSE 1688

CMD ["python", "/app/py-kms/server.py", ${server}, ${port} ]