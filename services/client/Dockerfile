FROM node:16-alpine

WORKDIR /usr/src/app

ENV PATH /usr/src/app/node_modules/.bin:$PATH

COPY package.json .
COPY package-lock.json .
RUN npm ci
RUN npm install react-scripts@4.0.3 prettier@2.3.0 -g --silent

CMD ["npm", "start"]