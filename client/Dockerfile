FROM node:18.19-alpine
WORKDIR /app
COPY . .
RUN npm install -g @angular/cli && npm install
CMD ["ng", "serve", "--host", "0.0.0.0"]
EXPOSE 4200
