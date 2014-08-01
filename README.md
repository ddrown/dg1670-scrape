dg1670-scrape
=============
 
Produce graphs from an Arris DG1670 cable modem

# Setup

1. have a dg1670 modem
2. setup your network so you are able to reach the modem's status interface via http://192.168.100.1
3. have perl modules CGI, HTML::TableExtract, RRDs (from rrdtool-perl in Fedora), LWP::UserAgent
4. create a directory /var/db/cable, writeable by a user of your choosing
5. run this script cable-modem from cron every 5 minutes as that user
6. put cablegraph in /var/www/cgi-bin or wherever your web server expects cgi programs
7. chmod 755 the cablegraph file

# Screenshot

![Cable Modem Status](cable-modem-screenshot.png?raw=true)
