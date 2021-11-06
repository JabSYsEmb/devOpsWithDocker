FROM ubuntu:18.04

WORKDIR /my/bin

RUN apt-get update && apt-get install -y curl python3 
RUN curl -L https://github.com/yt-dlp/yt-dlp/releases/download/2021.10.22/yt-dlp -o ./yt-dlp
RUN chmod +x yt-dlp

ENV LC_ALL=C.UTF-8

# CMD ["./yt-dlp"]

ENTRYPOINT yt-dlp
