# ベースとなるDockerイメージ指定
FROM golang:latest

WORKDIR /go/src

RUN apk update \
  && apk add --no-cache git \
  && go get github.com/gin-gonic/gin \
  && go get github.com/jinzhu/gorm \
  && go get github.com/go-sql-driver/mysql

EXPOSE 8080