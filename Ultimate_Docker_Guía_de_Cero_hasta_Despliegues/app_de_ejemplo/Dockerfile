FROM node:20.5.0-alpine3.18
WORKDIR /app/
COPY package*.json .
RUN npm install
COPY . .
ENV API=https://apiv1.miweb.com
EXPOSE 5173
RUN addgroup react && adduser -S -G react react
CMD ["npm", "run", "dev"]
