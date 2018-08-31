FROM golang

ENV PATH $PATH:$PATH/bin

#COPY . src/github.com/yulibaozi/yulibaozi.com/
COPY . /go_test
# ADD run.sh /

#WORKDIR /go/src/github.com/yulibaozi/yulibaozi.com

WORKDIR /go_test

# RUN chmod 777 ./run.sh

EXPOSE 8080


CMD ["./demo"]
