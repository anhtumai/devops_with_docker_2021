FROM node:14

WORKDIR /usr/src/app

COPY /material-applications/example-frontend /usr/src/app

RUN npm install

RUN npm run build

RUN npm install -g serve

EXPOSE 5000

CMD ["serve", "-s", "-l", "5000", "build"]

