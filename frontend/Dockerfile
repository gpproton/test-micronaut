# develop stage
FROM node:13.8-alpine as develop-stage
WORKDIR /app
COPY package*.json ./
RUN npm i -g @quasar/cli@latest
RUN npm i -g pm2@latest
COPY . .

# local-deps
FROM develop-stage as local-deps-stage
RUN yarn

# build stage
FROM local-deps-stage as build-stage
RUN quasar build -m ssr
CMD ["pm2-runtime", "dist/ssr/index.js"]

# dev stage
# FROM local-deps-stage as dev-stage
# RUN quasar dev -m ssr