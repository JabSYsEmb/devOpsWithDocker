FROM golang:1.16

WORKDIR /home/backend

COPY ./backend/ .

RUN go build

ENV REQUEST_ORIGIN=https://example.com
ENV PROT=8080

CMD ["./server"]
