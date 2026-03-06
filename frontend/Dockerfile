FROM node:18

WORKDIR /app

# enable yarn
RUN corepack enable

COPY package.json ./

RUN yarn install

COPY . .

EXPOSE 3000

CMD ["yarn","dev","--host","0.0.0.0"]