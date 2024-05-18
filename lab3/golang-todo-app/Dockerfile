FROM golang:alpine as builder
WORKDIR /app
COPY . . 
RUN go build -o main main.go


FROM alpine as prod
COPY --from=builder /app/main /bin/main
CMD [ "/bin/main" ]
RUN rm -rf /var/cache/apk/*
