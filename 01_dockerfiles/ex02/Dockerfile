FROM ruby
RUN apt update &&  apt -y upgrade && \ 
gem install rails && \
rails new APP
WORKDIR /APP
ENTRYPOINT rails server