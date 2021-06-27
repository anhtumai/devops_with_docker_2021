FROM alpine

WORKDIR /usr/src/app

COPY main.sh .

RUN chmod +x main.sh

RUN apk update; apk add curl

CMD ["sh" ,"./main.sh"]
