FROM node:16

WORKDIR /react/app

COPY . .

RUN npm i && npm run build

RUN mkdir -p /var/www/html
RUN mv build/* /var/www/html

WORKDIR /

RUN rm -rf /react/app
