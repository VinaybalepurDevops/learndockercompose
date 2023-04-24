FROM node:10
RUN mkdir servercode
COPY ./server /servercode
WORKDIR /servercode
ARG newip
RUN sed -i "s/ip/${newip}/g" db/index.js
RUN npm install -g  nodemon
RUN yarn install
CMD ["nodemon", "index.js"]
EXPOSE 3000
