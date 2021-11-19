FROM node:16
WORKDIR /usr/src/app
COPY package.json ./
RUN npm install -g serve && yarn install
COPY . .
RUN yarn build
CMD [ "serve", "-s", "build" ]