FROM debian

RUN apt update && apt -y install apache2 cpanminus libapache2-mod-perl2 libdbd-mysql-perl libtimedate-perl libnet-dns-perl libnet-ldap-perl libio-socket-ssl-perl libpdf-api2-perl libsoap-lite-perl libtext-csv-xs-perl libjson-xs-perl libapache-dbi-perl libxml-libxml-perl libxml-libxslt-perl libyaml-perl libarchive-zip-perl libcrypt-eksblowfish-perl libencode-hanextra-perl libmail-imapclient-perl libtemplate-perl libdatetime-perl libmoo-perl bash-completion libyaml-libyaml-perl libjavascript-minifier-xs-perl libcss-minifier-xs-perl libauthen-sasl-perl libauthen-ntlm-perl libhash-merge-perl libical-parser-perl libspreadsheet-xlsx-perl libcrypt-jwt-perl libcrypt-openssl-x509-perl jq cron nano libcpan-audit-perl libdata-uuid-perl wget && cpanm install Jq

ENV LINK=https://download.znuny.org/releases/znuny-latest-6.5.tar.gz
ENV VERSION=6.5.4

COPY ./script /usr/bin/script

EXPOSE 80

ENTRYPOINT /usr/bin/script