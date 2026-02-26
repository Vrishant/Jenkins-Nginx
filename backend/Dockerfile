FROM ubuntu:22.04

RUN apt-get update && apt-get install -y --no-install-recommends --fix-missing g++ libc6-dev

WORKDIR /app

COPY app.cpp .

RUN g++ app.cpp -o app

EXPOSE 8080

CMD ["./app"]