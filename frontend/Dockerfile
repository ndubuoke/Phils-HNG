FROM node:16-alpine 
WORKDIR /frontend
COPY package*.json ./
COPY . .
RUN npm i 
RUN npm run build
ENV NODE_ENV production
EXPOSE 3000
CMD ["npx", "src/index.js"]
# CMD [ "npx", "serve", "build" ]
# FROM node:19-alpine3.15
# WORKDIR /frontend
# COPY package*.json ./
# RUN npm install 
# COPY . .
# RUN npm run build
# EXPOSE 3000
# CMD ["npx", "serve", "build"]
