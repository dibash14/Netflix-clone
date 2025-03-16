FROM node:22 AS builder

WORKDIR /app

COPY . .

RUN npm i

FROM node:22-slim

WORKDIR /app

COPY --from=builder /app .

COPY config.env config.env

EXPOSE 5000

CMD ["npm","run","dev"]
