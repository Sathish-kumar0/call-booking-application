FROM node:17.9.0-slim
LABEL maintainer="sathish"
RUN useradd -m adminapi
WORKDIR /app
COPY . .
RUN npm install
RUN mkdir -p /home/adminapi && chown -R adminapi:adminapi /home/adminapi
EXPOSE 1004
USER adminapi
ENV MONGO_URL=""
CMD [ "npm", "start"]