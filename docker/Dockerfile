FROM ruby:latest

RUN gem install bundler
RUN gem install rails

# Install NodeJS
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb http://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list
RUN curl -sL https://deb.nodesource.com/setup_8.x | bash -
RUN apt install -y nodejs yarn

RUN gem install foreman

# Expose application port
EXPOSE 3000

# Expose API port
EXPOSE 3001
