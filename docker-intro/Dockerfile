FROM alpine:3.4
ADD . /usr/src/app/
WORKDIR /usr/src/app
RUN apk update && apk add nodejs
RUN apk add --update bash && rm -rf /var/cache/apk/*
RUN npm install -g reveal-md
EXPOSE 8000
CMD reveal-md docker-intro.md  --theme league -h 10.201.102.26 -p 8000
