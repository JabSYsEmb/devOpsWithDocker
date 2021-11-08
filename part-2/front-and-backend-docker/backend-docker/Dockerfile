FROM golang:1.16

WORKDIR /home/backend

COPY ./backend/ .

RUN go build

ENV REQUEST_ORIGIN=http://localhost:5002

ENV PORT=8080

CMD ["./server"]
