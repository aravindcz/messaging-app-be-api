FROM golang:1.21-alpine
WORKDIR /app
COPY . .
RUN go mod init worker && go mod tidy
RUN go build -o worker
CMD ["./worker"]