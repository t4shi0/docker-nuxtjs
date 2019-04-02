# イメージの指定
FROM node:lts-alpine

RUN npm install -g @vue/cli @vue/cli-service-global

WORKDIR /app



ENV HOST 0.0.0.0

EXPOSE 3000

# linuxを使う時のみuid gidを指定（ユーザー　グループ）
USER 1000:1000

