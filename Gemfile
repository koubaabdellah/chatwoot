source 'https://rubygems.org'

ruby '3.0.4'

##-- base gems for rails --##
gem 'rack-cors', require: 'rack/cors'
gem 'rails', '~> 6.1', '>= 6.1.7.3'
# Reduces boot times through caching; required in config/boot.rb
gem 'bootsnap', require: false

##-- rails application helper gems --##
gem 'acts-as-taggable-on'
gem 'attr_extras'
gem 'browser'
gem 'hashie'
gem 'jbuilder'
gem 'kaminari'
gem 'responders'
gem 'rest-client'
gem 'telephone_number'
gem 'time_diff'
gem 'tzinfo-data'
gem 'valid_email2'
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
gem 'rack-attack'
# a utility tool for streaming, flexible and safe downloading of remote files
gem 'down', '~> 5.0'

##-- for active storage --##
gem 'aws-sdk-s3', require: false
gem 'azure-storage-blob', require: false
gem 'google-cloud-storage', require: false
gem 'image_processing', '~> 1.12.2'

##-- gems for database --#
gem 'groupdate'
gem 'pg'
gem 'redis'
gem 'redis-namespace'
# super fast record imports in bulk
gem 'activerecord-import'

##--- gems for server & infra configuration ---##
gem 'dotenv-rails'
gem 'foreman'
gem 'puma'
gem 'webpacker', '~> 5.4', '>= 5.4.3'
# metrics on heroku
gem 'barnes'

##--- gems for authentication & authorization ---##
gem 'devise'
gem 'devise-secure_password', '~> 2.0', git: 'https://github.com/chatwoot/devise-secure_password'
gem 'devise_token_auth'
# authorization
gem 'jwt'
gem 'pundit'
# super admin
gem 'administrate'

##--- gems for pubsub service ---##
# https://karolgalanciak.com/blog/2019/11/30/from-activerecord-callbacks-to-publish-slash-subscribe-pattern-and-event-driven-design/
gem 'wisper', '2.0.0'

##--- gems for channels ---##
# TODO: bump up gem to 2.0
gem 'facebook-messenger'
gem 'line-bot-api'
gem 'twilio-ruby', '~> 5.66'
# twitty will handle subscription of twitter account events
# gem 'twitty', git: 'https://github.com/chatwoot/twitty'
gem 'twitty'
# facebook client
gem 'koala'
# slack client
gem 'slack-ruby-client'
# for dialogflow integrations
gem 'google-cloud-dialogflow'

##-- apm and error monitoring ---#
gem 'ddtrace'
gem 'elastic-apm'
gem 'newrelic_rpm'
gem 'scout_apm'
gem 'sentry-rails', '~> 5.3', '>= 5.3.1'
gem 'sentry-ruby', '~> 5.3'
gem 'sentry-sidekiq', '~> 5.3', '>= 5.3.1'

##-- background job processing --##
gem 'sidekiq', '~> 6.4.2'
# We want cron jobs
gem 'sidekiq-cron', '~> 1.6', '>= 1.6.0'

##-- Push notification service --##
gem 'fcm'
gem 'webpush'

##-- geocoding / parse location from ip --##
# http://www.rubygeocoder.com/
gem 'geocoder'
# to parse maxmind db
gem 'maxminddb'

# to create db triggers
gem 'hairtrigger'

gem 'procore-sift'

# parse email
gem 'email_reply_trimmer'
gem 'html2text'

# to calculate working hours
gem 'working_hours'

# full text search for articles
gem 'pg_search'

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
  gem 'bullet'
  gem 'letter_opener'
  gem 'web-console'

  # used in swagger build
  gem 'json_refs'

  # When we want to squash migrations
  gem 'squasher'
end

group :test do
  # Cypress in rails.
  gem 'cypress-on-rails', '~> 1.13', '>= 1.13.1'
  # fast cleaning of database
  gem 'database_cleaner'
  # mock http calls
  gem 'webmock'
end

group :development, :test do
  gem 'active_record_query_trace'
  ##--- gems for debugging and error reporting ---##
  # static analysis
  gem 'brakeman'
  gem 'bundle-audit', require: false
  gem 'byebug', platform: :mri
  gem 'climate_control'
  gem 'factory_bot_rails'
  gem 'listen'
  gem 'mock_redis'
  gem 'pry-rails'
  gem 'rspec_junit_formatter'
  gem 'rspec-rails', '~> 5.0.3'
  gem 'rubocop', require: false
  gem 'rubocop-performance', require: false
  gem 'rubocop-rails', require: false
  gem 'rubocop-rspec', require: false
  gem 'seed_dump'
  gem 'shoulda-matchers'
  gem 'simplecov', '0.17.1', require: false
  gem 'spring'
  gem 'spring-watcher-listen'
end
