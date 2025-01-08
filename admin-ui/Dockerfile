FROM node:17.9.0-slim
LABEL maintainer="sathish"
RUN useradd -m adminui
WORKDIR /app
COPY . .
RUN npm install
RUN mkdir -p /home/adminui && chown -R userapi:userapi /home/adminui
EXPOSE 3000
USER adminui
CMD [ "npm", "start"]
