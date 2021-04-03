FROM node:15-slim

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY ./package*.json ./

RUN npm install 
RUN npm run data:import

COPY . .

# Exports
EXPOSE 5000

CMD ["npm","start"]