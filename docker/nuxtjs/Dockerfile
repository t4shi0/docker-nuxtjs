# イメージの指定
FROM node:lts-alpine

WORKDIR /app

RUN yarn add nuxt -D
# RUN npm install --save-dev nuxt

ENV CHOKIDAR_USEPOLLING=true

# ホストがlinuxの場合のみownerがrootになるので対策（1000はホストubuntu uid）
# mac windowsは必要なし
#USER 1000

ENV HOST 0.0.0.0

EXPOSE 3000 3001



