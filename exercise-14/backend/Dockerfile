FROM golang:1.16

EXPOSE 8080

WORKDIR ~/backend-exercise

COPY . .

RUN go build

ENV REQUEST_ORIGIN=http://localhost:5000

RUN go test ./...

CMD ["./server"]