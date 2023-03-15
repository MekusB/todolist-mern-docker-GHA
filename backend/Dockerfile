FROM node:lts-buster-slim

# Create app directory
WORKDIR /usr/src/app

COPY backend/package.json /usr/src/app/package.json
COPY backend/package-lock.json /usr/src/app/package-lock.json
RUN npm ci

COPY . /usr/src/app

EXPOSE 3000

CMD [ "npm", "run", "dev" ]
