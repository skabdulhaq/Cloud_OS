FROM node:21-alpine3.18
WORKDIR /var/www
COPY . .
RUN npm install
RUN npm run build
ENV NODE_ENV=production
ENV HOST 0.0.0.0
EXPOSE 3000
CMD ["node", ".output/server/index.mjs"]
