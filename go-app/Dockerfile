FROM golang:1.22.2-alpine

WORKDIR /go/src/app

# Use COPY instead of ADD for better practices
COPY . .

# Combine RUN commands to reduce layers
RUN  go mod init && go build -o helloworld

EXPOSE 6111

CMD ["./helloworld"]