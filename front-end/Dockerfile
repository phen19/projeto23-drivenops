FROM node:16.14

WORKDIR /app

COPY . .

RUN npm i

RUN mkdir -p /var/www/html

RUN npm run build

RUN mv public /var/www/html

RUN mv build/* /var/www/html

WORKDIR /

RUN rm -rf /app
