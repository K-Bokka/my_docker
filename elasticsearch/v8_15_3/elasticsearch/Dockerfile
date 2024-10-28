FROM docker.elastic.co/elasticsearch/elasticsearch:8.15.3

WORKDIR "/usr/share/elasticsearch"
RUN ["bin/elasticsearch-plugin", "install", "analysis-kuromoji"]
RUN ["bin/elasticsearch-plugin", "install", "analysis-icu"]
