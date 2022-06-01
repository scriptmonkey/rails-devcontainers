FROM ruby:3.1.2-bullseye

RUN curl -s https://deb.nodesource.com/gpgkey/nodesource.gpg.key | gpg --dearmor | tee /usr/share/keyrings/nodesource.gpg >/dev/null \
  && echo 'deb [signed-by=/usr/share/keyrings/nodesource.gpg] https://deb.nodesource.com/node_16.x bullseye main' > /etc/apt/sources.list.d/nodesource.list \
  && echo 'deb-src [signed-by=/usr/share/keyrings/nodesource.gpg] https://deb.nodesource.com/node_16.x bullseye main' >> /etc/apt/sources.list.d/nodesource.list \
  && apt-get update \
  && apt-get install -y nodejs postgresql-client\
  && rm -rf  /var/lib/apt/lists/* \
  && gem install rails


