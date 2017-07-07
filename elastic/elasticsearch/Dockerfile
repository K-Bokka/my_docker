FROM elasticsearch:5.4.3-alpine

WORKDIR "/usr/share/elasticsearch"
RUN ["bin/elasticsearch-plugin", "install", "analysis-kuromoji"]
