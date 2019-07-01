#!/bin/sh
ARG ELK_VERSION

# https://github.com/elastic/elasticsearch-docker
FROM docker.elastic.co/elasticsearch/elasticsearch-oss:${ELK_VERSION}
RUN bin/elasticsearch-certutil cert | echo "config/elastic-certificates.p12"
#FROM docker.elastic.co/elasticsearch/elasticsearch-oss:6.6.0
#RUN bin/elasticsearch-plugin install -b com.floragunn:search-guard-6:6.6.0-24.1

#RUN chmod +x /usr/share/elasticsearch/plugins/search-guard-6/tools/install_demo_configuration.sh 
#RUN /usr/share/elasticsearch/plugins/search-guard-6/tools/install_demo_configuration.sh -y
#ENTRYPOINT service elasticsearch restart
#RUN /usr/share/elasticsearch/plugins/search-guard-6/tools/sgadmin_demo.sh

#RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install x-pack --batch

# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
