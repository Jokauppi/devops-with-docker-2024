FROM ubuntu:22.04

EXPOSE 4173

WORKDIR /usr/src/app

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_20.x | bash
RUN apt install -y nodejs

COPY . .

RUN npm install

RUN npm run build

CMD npm run preview -- --host
