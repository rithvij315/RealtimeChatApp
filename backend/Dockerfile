FROM golang:1.11.1-alpine3.8
RUN apk add bash ca-certificates git gcc g++ libc-dev
RUN mkdir /app
ADD . /app/
WORKDIR /app
RUN go mod download
RUN go build -v
EXPOSE 8080
CMD ["/app/realtime-chat-go-react"]