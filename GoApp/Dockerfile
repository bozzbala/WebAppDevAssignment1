# Dockerfile
#FROM golang:1.20 AS builder
#WORKDIR /app
#COPY go.mod ./
#COPY main.go ./
#RUN go build -o hello-world .
#FROM alpine:latest
#WORKDIR /app
#COPY --from=builder /app/hello-world .
#ENTRYPOINT ["./hello-world"]

# Single-stage Dockerfile
FROM golang:1.20
WORKDIR /app
COPY go.mod ./
COPY main.go .
RUN go build -o hello-world .
ENTRYPOINT ["./hello-world"]
