FROM busybox:stable
WORKDIR /srv
COPY mypage/ .
RUN cp health.html health
# RUN printf "ok\n" > health
EXPOSE 8080
CMD ["sh", "-c", "httpd -f -p 8080 -h /srv"]