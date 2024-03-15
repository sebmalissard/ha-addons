ARG BUILD_FROM=alpine:latest
FROM $BUILD_FROM

RUN apk add --no-cache nginx

COPY website.conf /etc/nginx/http.d/default.conf

RUN mkdir -p /data/site 

EXPOSE 80

USER nginx
CMD ["nginx", "-g", "daemon off;"]
