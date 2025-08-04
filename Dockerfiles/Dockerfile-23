FROM nginx

#COPY default.conf /etc/nginx/conf.d/default.conf
RUN sed -i 's/^\s*listen\s*80;/listen 180;/g' /etc/nginx/conf.d/default.conf && \
   sed -i 's/^\s*listen\s*\[::\]:80;/listen [::]:180;/g' /etc/nginx/conf.d/default.conf
   
EXPOSE 180

CMD ["nginx", "-g", "daemon off;"]

