FROM node:8

RUN mkdir -p /var/www/app

WORKDIR /var/www/app

COPY package.json /var/www/app

RUN npm install

RUN npm install -g nodemon

COPY . /var/www/app

EXPOSE 3000

CMD ["npm", "start"]