FROM node:10
RUN mkdir clientcode
COPY ./client /clientcode
WORKDIR /clientcode
RUN cd /clientcode
RUN yarn install
ARG newip
RUN sed -i "s/ip/${newip}/g" src/api/index.js
CMD [ "yarn", "start" ]
EXPOSE 8000
