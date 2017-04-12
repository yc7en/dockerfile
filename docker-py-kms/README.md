py-kms Dockerfile
============================

This image provide a kms server written in python. It supports activating Windows 7/8/8.1/2008R2/2012/2012R2 and Office 2010/2013. Sourcecode is available at Github [myanaloglife/py-kms](https://github.com/myanaloglife/py-kms).

Useage
------------------------------

Simply,you can run the image directly:
 
	$ docker run -d -p 1688:1688 yc7en/py-kms

Then server run on http://your_dockerip:1688. Or you want run on any other port. You can run like this:

	$ docker run -d -p your_port:1688 yc7en/py-kms

