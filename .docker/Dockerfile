FROM squidfunk/mkdocs-material as build
COPY . . 
RUN mkdocs build --clean --site-dir /site

# serve the site
FROM nginx:alpine
COPY --from=build /site /usr/share/nginx/html
COPY .docker/nginx.conf /etc/nginx/conf.d/default.conf