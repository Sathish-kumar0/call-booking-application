FROM node:17.9.0-slim
LABEL maintainer="sathish"
RUN useradd -m userapi
WORKDIR /app
COPY . .
RUN npm install
RUN mkdir -p /home/userapi && chown -R userapi:userapi /home/userapi
EXPOSE 1004
USER userapi
ENV MONGO_URL=""
ENV ADMIN_EMAIL=""
CMD [ "npm", "start"]