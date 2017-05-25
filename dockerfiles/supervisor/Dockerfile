FROM puneeth-sshd

RUN apt-get update && apt-get install -y supervisor

RUN mkdir -p /var/log/supervisor

ADD ./supervisord.conf /etc/supervisor/supervisord.conf

EXPOSE 22

CMD ["/usr/bin/supervisord","-c","/etc/supervisor/supervisord.conf"]
