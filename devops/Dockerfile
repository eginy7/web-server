FROM node:10.16-alpine

ENV TERM=xterm

RUN apk add --no-cache git && git clone https://github.com/eginy7/web-server.git /app \
    && cd /app && npm install pm2@latest -g && npm install 

CMD ["pm2-runtime", "/app/src/app.js"]