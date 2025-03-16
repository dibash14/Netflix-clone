#first stage______________________
FROM node:16 AS frontend-builder

WORKDIR /app

COPY . .

RUN npm install --legacy-peer-deps 


COPY  .env .env

CMD ["npm","start"]
