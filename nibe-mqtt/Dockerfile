ARG BUILD_FROM
FROM $BUILD_FROM

RUN apk add --no-cache python3 py3-pip

RUN pip3 install nibe-mqtt==0.3.1

COPY run.sh /home
RUN chmod a+x /home/run.sh

COPY config_example.yaml /home/config_example.yaml

CMD [ "/home/run.sh" ]

