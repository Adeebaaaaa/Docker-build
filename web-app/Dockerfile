# go-service/Dockerfile

# ---- Build Stage ----
FROM golang:1.22-alpine AS builder

WORKDIR /app

# Create a simple Go program
RUN echo 'package main

RUN go build -o app main.go

# ---- Runtime Stage ----
FROM alpine:3.19

WORKDIR /app
COPY --from=builder /app/app .

EXPOSE 8080

CMD ["./app"]