FROM ruby:3.1-slim

RUN apt-get update && \
    apt-get install -y build-essential default-mysql-client default-libmysqlclient-dev git libvips-dev

WORKDIR /opt/back
COPY src/Gemfile src/Gemfile.lock ./
RUN bundle install

COPY entrypoint.sh /
RUN chmod +x /entrypoint.sh

ENTRYPOINT [ "/entrypoint.sh" ]
CMD [ "rails", "server", "-b", "0.0.0.0" ]
