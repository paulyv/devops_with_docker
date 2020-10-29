FROM ruby:2.6.0

WORKDIR /app

ADD ./rails-example-project-master .
RUN  apt-get update && apt-get install -y nodejs
RUN bundle update --bundler
RUN bundle install
RUN rails db:migrate RAILS_ENV=development

CMD ["rails", "s"]
