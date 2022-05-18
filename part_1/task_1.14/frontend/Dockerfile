FROM ubuntu:latest

WORKDIR /usr/src

COPY . .

ENV REACT_APP_BACKEND_URL http://localhost:8080/

RUN apt update && apt install -y curl && curl https://deb.nodesource.com/setup_16.x | apt install -y nodejs

RUN apt install -y npm && npm install 

RUN npm run build && npm install -g serve

EXPOSE 5000

CMD ["npx", "serve", "-s", "-l", "5000", "build"]
