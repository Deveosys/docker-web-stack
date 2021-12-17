
FROM node:16-alpine3.11

# this is a development Dockerfile
# and is not intended for production use
WORKDIR /var/www/nextjs

COPY package.json /var/www/nextjs/
COPY yarn.lock /var/www/nextjs/
RUN yarn install

COPY . /var/www/nextjs

# this what make hot reloading works
# because you are starting your project
# in the same way you running it locally
# CMD yarn dev