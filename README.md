# What is this?

This is a bash script around openssl, to make interrogation of ssl certification information easier.

It's basically a copy of [Alain Kelder's certify.sh bash script](http://giantdorks.org/alain/shell-script-to-check-ssl-certificate-info-like-expiration-date-and-subject/), and all credit goes to Alain; we simply make available here so that it's easier to install it directly using curl:

    curl https://raw.githubusercontent.com/jcdarwin/certify/master/certify.sh > certify \
    	&& chmod ug+x certify \
    	&& ./certify --help

My most-used application of this script is to see the validity of the cert for a given domain:

    ./certify --host github.com --dates
