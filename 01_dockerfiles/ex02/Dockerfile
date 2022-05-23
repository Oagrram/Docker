FROM ruby

RUN apt update &&  apt -y upgrade  && apt -y install sqlite3  && apt -y  install nodejs && gem install rails

ONBUILD COPY app /opt/app

ONBUILD WORKDIR /opt/app

ONBUILD RUN bundle install

# docker build  -t ft-rails:on-build . 
# copy app from docker help 
# docker build -t last -f Dockerfile-build  .
# docker run -it --rm -p 3000:3000 last