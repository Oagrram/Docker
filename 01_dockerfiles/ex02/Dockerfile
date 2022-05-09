FROM ruby
RUN apt update &&  apt -y upgrade  && apt -y install sqlite3  && apt -y  install nodejs && gem install rails
ONBUILD COPY app /opt/app
ONBUILD WORKDIR /opt/app
ONBUILD RUN bundle install

#docker build  -t ft-rails:on-build . 
