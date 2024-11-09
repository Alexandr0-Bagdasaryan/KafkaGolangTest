# syntax=docker/dockerfile:1

FROM golang:1.21

WORKDIR /api-gateway

COPY go.mod go.sum ./

RUN go mod download

COPY *.go ./

RUN go build -o /api-gateway

CMD ["./api-gateway"]