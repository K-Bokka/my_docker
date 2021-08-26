FROM amazon/opendistro-for-elasticsearch:1.13.2

RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch analysis-kuromoji
RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch analysis-icu
RUN /usr/share/elasticsearch/bin/elasticsearch-plugin remove opendistro_security
