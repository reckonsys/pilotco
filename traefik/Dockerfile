FROM traefik:v2.3
EXPOSE 443
RUN mkdir -p /etc/traefik/acme
RUN touch /etc/traefik/acme/acme.json
RUN chmod 600 /etc/traefik/acme/acme.json
COPY traefik.toml /etc/traefik
COPY services.toml /etc/traefik
# Custom SSL Certificate
# COPY /path/to/ssl.crt /certs/ssl.crt
# COPY /path/to/ssl.key /certs/ssl.key
# CMD traefik
