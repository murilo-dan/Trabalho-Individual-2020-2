FROM node:14.16.1

WORKDIR /app

COPY package*.json ./

RUN yarn global add @quasar/cli
RUN yarn install

COPY . .

CMD yarn && quasar dev