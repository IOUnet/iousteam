# Stage 0, "build-stage", based on Node.js, to build and compile the frontend
FROM node:16 
# as build-stage 

# WORKDIR /app

# COPY package*.json ./

# COPY ./node_modules/ ./
COPY . .
# RUN yarn install

# RUN yarn dev
# EXPOSE 3000
CMD npm run  dev

# WORKDIR /app/dist
# Stage 1, based on Nginx, to have only the compiled app, ready for production with Nginx
# FROM nginx:1

# COPY --from=build-stage /app/dist/ /usr/share/nginx/html

# COPY ./nginx.conf /etc/nginx/conf.d/default.conf
# COPY ./nginx-backend-not-found.conf /etc/nginx/extra-conf.d/backend-not-found.conf
