FROM ubuntu:22.04

WORKDIR /usr/app/src

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash
RUN apt-get install -y nodejs

ENV REACT_APP_BACKEND_URL=http://localhost:8080

COPY . .

RUN npm install

COPY . .

RUN npm run build

RUN npm install -g serve

EXPOSE 5000

CMD ["serve", "-s", "-l", "5000", "build"]
