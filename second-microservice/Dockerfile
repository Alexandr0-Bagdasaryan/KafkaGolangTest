# syntax=docker/dockerfile:1

FROM golang:1.21

WORKDIR /second-microservice

COPY go.mod go.sum ./

RUN go mod download

COPY *.go ./

RUN go build -o /second-microservice

CMD ["./second-microservice"]