FROM ubuntu:22.04

RUN apt -y update && apt -y install curl

RUN curl --proto '=https' --tlsv1.2 -sSf https://tiup-mirrors.pingcap.com/install.sh | sh && ln -s /root/.tiup/bin/tiup /bin/tiup

ENV TIDB_VERSION=v7.1.1
ENV DATA_DIR=v7_1_1

RUN tiup install tidb:${TIDB_VERSION} pd:${TIDB_VERSION} tikv:${TIDB_VERSION} prometheus:${TIDB_VERSION} grafana:${TIDB_VERSION} playground

CMD tiup playground ${TIDB_VERSION} --tag ${DATA_DIR} --db.host 0.0.0.0 --pd.host 0.0.0.0 --tiflash 0
