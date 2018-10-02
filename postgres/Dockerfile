FROM postgres:10.5

MAINTAINER Victor Lin <victor.lin@kkday.com>

RUN apt update
RUN apt install -y net-tools vim python python-psycopg2 ssh
RUN echo "root:root" | chpasswd

COPY sshd_config /etc/ssh/

EXPOSE 5022
EXPOSE 5432

CMD ["postgres"];docker-entrypoint.sh postgres