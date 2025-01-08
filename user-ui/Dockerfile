FROM node:17.9.0-slim
LABEL maintainer="sathish"
RUN useradd -m userui
WORKDIR /app
COPY . .
RUN mkdir -p /home/userui && chown -R userapi:userapi /home/userui
RUN npm install
EXPOSE 3000
USER userui
CMD [ "npm", "start"]
