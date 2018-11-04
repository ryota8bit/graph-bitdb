FROM node:8.9.4-alpine

RUN \
  apk update && \
  apk add git wget tar make g++ bash && \
  apk add --update python

# RUN npm config set python /usr/bin/python2.7

ENV APP_ROOT=/app
RUN mkdir -p ${APP_ROOT}
WORKDIR ${APP_ROOT}
RUN git clone https://github.com/21centurymotorcompany/bitd.git

WORKDIR ${APP_ROOT}/bitd
ADD ./containers/bitdb/config.js .
RUN chmod +x ./config.js
RUN npm install
CMD ["npm", "start"]
