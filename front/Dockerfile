FROM node:17.8.0-slim

USER node
WORKDIR /opt/front

COPY ./package.json ./yarn.lock ./
RUN yarn cache clean && yarn install

# MEMO: production では yarn start かも ...
CMD [ "yarn", "dev" ]
