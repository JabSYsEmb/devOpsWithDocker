FROM ruby:3.0.0

WORKDIR ./app

COPY ./rails-project/. .

RUN apt-get update 

RUN apt-get install -y nodejs

RUN apt-get install -y npm

RUN npm install -g yarn 

RUN gem install bundler:2.2.11

RUN bundle install

RUN rails db:migrate RAILS_ENV=production

RUN rake assets:precompile

CMD ["rails","s","-e","production"]
