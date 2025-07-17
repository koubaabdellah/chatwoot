source 'https://rubygems.org'

ruby '3.0.4'

##-- base gems for rails --##
gem 'rack-cors', '>= 2.0.0', require: 'rack/cors'
gem 'rails', '~> 7.1', '>= 7.1.0'
# Reduces boot times through caching; required in config/boot.rb
gem 'bootsnap', require: false

##-- rails application helper gems --##
gem 'acts-as-taggable-on'
gem 'attr_extras'
gem 'browser'
gem 'hashie'
gem 'jbuilder', '>= 2.12.0'
gem 'kaminari'
gem 'responders', '>= 3.1.0'
gem 'rest-client'
gem 'telephone_number'
gem 'time_diff'
gem 'tzinfo-data'
gem 'valid_email2', '>= 4.0.4'
# compress javascript config.assets.js_compressor
gem 'uglifier'
##-- used for single column multiple binary flags in notification settings/feature flagging --##
gem 'flag_shih_tzu'
# Random name generator for user names
gem 'haikunator'
# Template parsing safely
gem 'liquid'
# Parse Markdown to HTML
gem 'commonmarker'
# Validate Data against JSON Schema
gem 'json_schemer'
# Rack middleware for blocking & throttling abusive requests
gem 'rack-attack', '>= 6.7.0'
# a utility tool for streaming, flexible and safe downloading of remote files
gem 'down', '~> 5.0'

##-- for active storage --##
gem 'aws-sdk-s3', require: false
gem 'azure-storage-blob', require: false
gem 'google-cloud-storage', '>= 1.43.0', require: false
gem 'image_processing', '~> 1.12.2'

##-- gems for database --#
gem 'groupdate'
gem 'pg'
gem 'redis'
gem 'redis-namespace'
# super fast record imports in bulk
gem 'activerecord-import', '>= 1.4.1'

##--- gems for server & infra configuration ---##
gem 'dotenv-rails', '>= 2.8.0'
gem 'foreman'
gem 'puma'
gem 'webpacker', '~> 5.4', '>= 5.4.4'
# metrics on heroku
gem 'barnes'

##--- gems for authentication & authorization ---##
gem 'devise', '>= 4.9.0'
gem 'devise-secure_password', '~> 2.0', git: 'https://github.com/chatwoot/devise-secure_password'
gem 'devise_token_auth', '>= 1.2.3'
# authorization
gem 'jwt'
gem 'pundit', '>= 2.3.0'
# super admin
gem 'administrate', '>= 0.18.0'

##--- gems for pubsub service ---##
# https://karolgalanciak.com/blog/2019/11/30/from-activerecord-callbacks-to-publish-slash-subscribe-pattern-and-event-driven-design/
gem 'wisper', '2.0.0'

##--- gems for channels ---##
# TODO: bump up gem to 2.0
gem 'facebook-messenger'
gem 'line-bot-api'
gem 'twilio-ruby', '~> 5.69', '>= 5.69.0'
# twitty will handle subscription of twitter account events
# gem 'twitty', git: 'https://github.com/chatwoot/twitty'
gem 'twitty'
# facebook client
gem 'koala', '>= 3.3.0'
# slack client
gem 'slack-ruby-client'
# for dialogflow integrations
gem 'google-cloud-dialogflow', '>= 1.6.0'

##-- apm and error monitoring ---#
gem 'ddtrace'
gem 'elastic-apm'
gem 'newrelic_rpm'
gem 'scout_apm'
gem 'sentry-rails', '~> 5.4', '>= 5.4.0'
gem 'sentry-ruby', '~> 5.3'
gem 'sentry-sidekiq', '~> 5.4', '>= 5.4.0'

##-- background job processing --##
gem 'sidekiq', '~> 6.5.0'
# We want cron jobs
gem 'sidekiq-cron', '~> 1.7', '>= 1.7.0'

##-- Push notification service --##
gem 'fcm'
gem 'webpush'

##-- geocoding / parse location from ip --##
# http://www.rubygeocoder.com/
gem 'geocoder'
# to parse maxmind db
gem 'maxminddb'

# to create db triggers
gem 'hairtrigger', '>= 1.0.0'

gem 'procore-sift', '>= 1.0.0'

# parse email
gem 'email_reply_trimmer'
gem 'html2text', '>= 0.4.0'

# to calculate working hours
gem 'working_hours', '>= 1.5.0'

# full text search for articles
gem 'pg_search', '>= 2.3.7'

# Subscriptions, Billing
gem 'stripe'

## - helper gems --##
## to populate db with sample data
gem 'faker'

group :production, :staging do
  # we dont want request timing out in development while using byebug
  gem 'rack-timeout'
end

group :development do
  gem 'annotate'
  gem 'bullet', '>= 7.0.3'
  gem 'letter_opener'
  gem 'web-console', '>= 4.2.1'

  # used in swagger build
  gem 'json_refs'

  # When we want to squash migrations
  gem 'squasher'
end

group :test do
  # Cypress in rails.
  gem 'cypress-on-rails', '~> 1.14', '>= 1.14.0'
  # fast cleaning of database
  gem 'database_cleaner', '>= 2.0.2'
  # mock http calls
  gem 'webmock', '>= 3.15.1'
end

group :development, :test do
  gem 'active_record_query_trace'
  ##--- gems for debugging and error reporting ---##
  # static analysis
  gem 'brakeman'
  gem 'bundle-audit', require: false
  gem 'byebug', platform: :mri
  gem 'climate_control'
  gem 'factory_bot_rails', '>= 6.3.0'
  gem 'listen'
  gem 'mock_redis'
  gem 'pry-rails'
  gem 'rspec_junit_formatter'
  gem 'rspec-rails', '~> 5.1.0'
  gem 'rubocop', require: false
  gem 'rubocop-performance', require: false
  gem 'rubocop-rails', '>= 2.16.0', require: false
  gem 'rubocop-rspec', require: false
  gem 'seed_dump'
  gem 'shoulda-matchers', '>= 5.2.0'
  gem 'simplecov', '0.17.1', require: false
  gem 'spring'
  gem 'spring-watcher-listen'
end
