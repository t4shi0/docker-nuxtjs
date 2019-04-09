# イメージの指定
FROM node:lts-alpine

WORKDIR /app

RUN npm install --save-dev nuxt

# ホストがlinuxの場合のみownerがrootになるので対策（1000はホストubuntu uid）
# mac windowsは必要なし
USER 1000

ENV HOST 0.0.0.0

EXPOSE 3000

WORKDIR /app/nuxt_project


