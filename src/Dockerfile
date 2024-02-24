FROM golang:1.21.6

WORKDIR /server

COPY . .

RUN go mod download

COPY . .

RUN go build -o echo-server .

EXPOSE 1323

CMD ["./echo-server"]