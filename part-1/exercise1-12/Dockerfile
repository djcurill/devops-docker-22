FROM ubuntu:latest

WORKDIR /usr/src/app

RUN apt update && apt install -y curl
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash
RUN apt-get install -y nodejs

COPY package* .

RUN npm install

COPY . .

RUN npm run build
RUN npm install -g serve

CMD ["serve","-s","-l","5000","build"]

EXPOSE 5000



