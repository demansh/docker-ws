FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
    apache2 \
    bash \
    && rm -rf /var/lib/apt/lists/*

EXPOSE 80

COPY index.html /var/www/html/index.html

CMD ["sh", "-c", "service apache2 start && bash"]
