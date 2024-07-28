FROM ontotext/graphdb:10.5.1@sha256:dd7d0a0c44bd57ddd1fcaf95442c38d7c561334d24bea2b28c8a600fc3e25cf3
RUN mkdir -p /opt/graphdb/dist/data/repositories/starwars
COPY config-starwars.ttl /opt/graphdb/dist/data/repositories/starwars/config.ttl
RUN mkdir -p /opt/graphdb/dist/data/repositories/langchain
COPY config-langchain.ttl /opt/graphdb/dist/data/repositories/langchain/config.ttl
COPY starwars-data.trig /
COPY berners-lee-card.ttl /
COPY graphdb_create.sh /run.sh
ENTRYPOINT bash /run.sh