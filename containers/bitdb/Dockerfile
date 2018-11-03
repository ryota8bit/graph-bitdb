FROM node:8.9.4-alpine

RUN set -x && \
  rm -rf /var/lib/apt/lists/* && \
  apt-get clean && \
  apt-get update \
  apt-get -y install git wget tar

ENV APP_ROOT=/app
RUN mkdir -p ${APP_ROOT}
WORKDIR ${APP_ROOT}
RUN git clone https://github.com/21centurymotorcompany/bitd.git
RUN npm install
# CMD ["npm", "start"]