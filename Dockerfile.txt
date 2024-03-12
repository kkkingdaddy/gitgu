FROM node:20-alpine

RUN apk add --no-cache git

RUN git clone https://github.com/Knikoni/math-homework.git

WORKDIR /math-homework

RUN npm install

CMD npm start
