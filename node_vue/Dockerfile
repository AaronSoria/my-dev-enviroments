FROM node:16-alpine
WORKDIR /app
RUN npm install -g @vue/cli
EXPOSE 8081:8080
ENV CHOKIDAR_USEPOLLING=true
CMD ["npm", "run", "serve"]