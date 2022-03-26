FROM golang:1.15-alpine

RUN apk update \
    && apk add --no-cache tzdata git ca-certificates make bash yarn nodejs

RUN go env -w GO111MODULE=on  \
    && go env -w GOPROXY=https://goproxy.cn,direct \
    && echo go version


WORKDIR /www

