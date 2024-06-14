
##### Stage 1

FROM ubuntu AS build

RUN apt-get update && apt-get install -y golang-go

ENV GO111MODULE=off

copy . .

RUN CGO_ENABLED=0 go build -o /app .

##### Stage 2

FROM scratch

COPY --from=build /app /app

ENTRYPOINT ["/app"]
