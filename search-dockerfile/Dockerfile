FROM jetty:9.3.10

MAINTAINER Robert Kaye <rob@metabrainz.org>

WORKDIR $JETTY_HOME
RUN curl -o $JETTY_HOME/webapps/ROOT.war http://ftp.musicbrainz.org/pub/musicbrainz/search/servlet/searchserver.war && apt-get update && apt-get install paxctl && paxctl -c /usr/bin/java && paxctl -m /usr/bin/java
