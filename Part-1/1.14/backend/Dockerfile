FROM golang:1.16.15-bullseye

EXPOSE 8080

WORKDIR /usr/src/app

COPY . .

RUN go build

ENV PORT=8080
ENV REQUEST_ORIGIN=http://localhost:5000

CMD ["./server"]
