FROM litaio/ruby:2.3.0
MAINTAINER Jimmy Cuadra <jimmy@jimmycuadra.com>

RUN gem install bundler lita

RUN lita new app

WORKDIR /app

COPY config/lita_config.rb lita_config.rb

COPY config/Gemfile Gemfile 

COPY config/start /start

CMD ["/start"]
