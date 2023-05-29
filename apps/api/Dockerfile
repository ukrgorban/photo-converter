FROM node:14.19.0-alpine3.14
WORKDIR /opt/app
ADD *.json ./
RUN npm install
ADD . .
RUN npm run build api
CMD ["node", "./dist/apps/api/main.js"]
