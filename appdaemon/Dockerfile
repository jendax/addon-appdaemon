ARG BUILD_FROM
FROM $BUILD_FROM

ENV LANG C.UTF-8

RUN apk add --no-cache python3 py3-pip && \
    pip3 install appdaemon==4.0.6

COPY run.sh /run.sh
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]