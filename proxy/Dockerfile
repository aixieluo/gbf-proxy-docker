FROM golang:latest

WORKDIR /go/src/

COPY ./gbf_proxy ./gbf_proxy

COPY ./build.sh ./build.sh

EXPOSE 8088

CMD ["/bin/bash", "/go/src/build.sh"]
