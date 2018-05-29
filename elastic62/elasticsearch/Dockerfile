FROM docker.elastic.co/elasticsearch/elasticsearch:6.2.4

WORKDIR "/usr/share/elasticsearch"
RUN ["bin/elasticsearch-plugin", "install", "analysis-kuromoji"]
RUN ["bin/elasticsearch-plugin", "install", "analysis-icu"]
