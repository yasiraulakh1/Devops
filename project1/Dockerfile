# Stage 1: Build NGINX with Custom HTML
FROM nginx:alpine AS build
WORKDIR /usr/share/nginx/html
RUN echo "Hello, World!" > index.html

# Stage 2: Final Image
FROM nginx:alpine
COPY --from=build /usr/share/nginx/html /usr/share/nginx/html

