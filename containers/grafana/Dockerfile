FROM grafana/grafana

RUN apt-get install git nodejs npm

WORKDIR /var/lib/grafana/plugins
RUN git clone https://github.com/JamesOsgood/mongodb-grafana
