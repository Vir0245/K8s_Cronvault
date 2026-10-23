FROM nginx:1.27
# Copy nginx config that works without TLS certs for basic ECR build
COPY nginx.conf /etc/nginx/conf.d/default.conf
# Bake the dashboard directly (build context has index.html)
COPY index.html /usr/share/nginx/html/index.html
EXPOSE 80 443
