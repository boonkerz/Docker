FROM maxexcloo/debian:latest
MAINTAINER Thomas Peterson <info@thomas-peterson.de>
ENV VERSION 0.3.3
RUN wget -O - "https://www.github.com/jwilder/docker-gen/releases/download/${VERSION}/docker-gen-linux-amd64-${VERSION}.tar.gz" | tar -C /usr/local/bin -x -z
ADD config /config
ADD supervisord.conf /etc/supervisor/conf.d/docker-gen.conf
