FROM node:current-buster

# Clone ciscc-api
RUN git clone --depth=1 https://github.com/pan93412/ciscc-api /app && \
    chmod -R 0777 /app
WORKDIR /app

# Install and build
RUN yarn && yarn build

CMD yarn start:prod
