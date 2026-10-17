FROM node:20
WORKDIR /app
COPY . .
RUN npm install
RUN npm run build
RUN apt-get update -y && apt-get install -y nginx
RUN rm -rf /var/www/html/*
RUN cp -r /app/dist/* /var/www/html/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
