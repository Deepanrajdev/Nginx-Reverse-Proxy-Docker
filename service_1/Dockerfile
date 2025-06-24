FROM golang:1.19
WORKDIR /app
 
COPY . .

RUN go build -o service1 main.go

EXPOSE 8001

CMD ["go","run","main.go"]

#go run main.go