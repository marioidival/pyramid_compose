FROM golang:1.5-wheezy

RUN curl -sL https://deb.nodesource.com/setup_4.2.4 | bash -
RUN apt-get --yes --quiet install --no-install-recommends\
	nodejs \
 	npm \
    && rm -rf /var/lib/apt/lists/*
RUN npm install -g bower
RUN go get -u -v github.com/mholt/caddy
RUN go install github.com/mholt/caddy
RUN which caddy

ADD . /site/frontend
WORKDIR /site/frontend
RUN bower install --allow-root

EXPOSE 2015
CMD ["/go/bin/caddy"]
