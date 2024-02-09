FROM node:16-alpine
RUN mkdir -p /app
WORKDIR /app
COPY ./ .
ENV REACT_APP_BACKEND_WS=ws://localhost:8080
ENV REACT_APP_BACKEND_URL=http://localhost:8080
ENV REDIS_ADDR=Docker-Redis:6379
ENV ALLOWED_ORIGIN=http://localhost:3000
RUN npm install
RUN npm install -g serve
RUN npm run build
EXPOSE 3000
CMD ["serve", "-s", "build", "-l", "3000"]