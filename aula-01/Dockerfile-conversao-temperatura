FROM node
WORKDIR /app
COPY ./conversao-temperatura/src/package*.json ./
RUN npm install
COPY ./conversao-temperatura/src .
CMD ["npm", "run", "start"]
