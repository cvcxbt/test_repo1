source 'https://rubygems.org'
ruby '2.2.3'

gem 'rails', '4.2.5'
gem 'jbuilder'

gem 'pg'
gem 'activerecord-postgis-adapter'

# Using composite primary keys for RETS associations
gem 'composite_primary_keys'

gem 'haml-rails'

# Assets
gem 'coffee-rails'
gem 'sass-rails'
gem 'bourbon'
gem 'uglifier'

gem 'jquery-rails'
gem 'jquery-ui-rails'
gem 'jquery-validation-rails'
gem 'jquery-fileupload-rails'
gem 'react-rails', github: 'reactjs/react-rails'
gem 'sprockets-coffee-react'

# Authorizations
gem 'devise'
gem 'devise_invitable'
gem 'omniauth-oauth2'

gem 'rack-attack'

# Utils
gem 'oj'
gem 'httparty'
gem 'state_machine'
gem 'will_paginate-bootstrap'
gem 'hashr', '~> 1.0'
gem 'handy', '0.0.28'

# For sending push notifications
gem 'grocer' # to iOS
gem 'gcm'    # to Android

# Background jobs processing
gem 'sidekiq'
gem 'sidekiq-unique-jobs', '~> 3.0'
gem 'sinatra' # Used by sidekiq WebUI

# SAML SSO
gem 'ruby-saml'
gem 'ruby-saml-idp', github: 'lawrencepit/ruby-saml-idp'

# External Services APIs

gem 'spark_api'

gem 'mandrill-api'
gem 'mandrill-rails'

gem 'gibbon'

gem 'twilio-ruby'

gem 'pubnub'
gem 'intercom'
gem 'intercom-rails'

# Rails Engine for Links Shortener logic
gem 'shortener'

# Profilers
gem 'newrelic_rpm'
gem 'honeybadger'

# Export
gem 'icalendar'
gem 'axlsx'
gem 'active_model_serializers'

# Caching

## Memcachier gem to setup Dali Client to connect Memcacheir Servers
gem 'memcachier'
## Memcached Client and their stuff
gem 'kgio'
gem 'dalli'

# Avatar uploading
gem 'aws-sdk', '< 2.0'
gem 'carrierwave'
gem 'mini_magick'
gem 'carrierwave-aws'

# Administrators panel
gem 'activeadmin', github: 'activeadmin'

gem 'analytics-ruby', require: 'segment/analytics'

# Using rets to communicate with RETS services
gem 'rets', github: 'estately/rets', ref: '08f1c4b1fb4efa0eec77fd698f0c56ae6c6df2f2'

# Using api-auth to safely authenticate callsupport
gem 'api-auth'

# Creating documentation for API
gem 'apipie-rails', github: 'Apipie/apipie-rails'

group :staging, :production do
  gem 'puma'
  gem 'rails_12factor'
  gem 'heroku-deflater'
  gem 'rack-cache'
  gem 'le'
end

group :staging, :development do
  gem 'sucker_punch'
end

group :development, :test do
  gem 'thin'

  # Rails Env preloader to speedup running rails server, tests and rake tasks
  gem 'spring', require: false
  gem 'spring-commands-testunit', require: false

  # Hide log entries on accessing assets
  gem 'quiet_assets'

  # Debug
  gem 'awesome_print'
  gem 'coolline'

  # Ruby Console
  gem 'pry'
  gem 'pry-byebug'

  # Profiling tools
  gem 'memory_profiler', require: false
  gem 'ruby-prof', require: false

  # Run tests by using all your CPU cores
  gem 'parallel_tests'
end

group :development do
  gem 'guard', require: false
  gem 'guard-livereload', require: false

  # Rails 4.2 web console
  gem 'web-console'

  # Server deployment
  gem 'capistrano'
  gem 'capistrano-rails'
  gem 'capistrano-bundler'
  gem 'capistrano-rbenv'
  gem 'net-ssh'
  gem 'j-cap-recipes'
end

group :test do
  # Sample data
  gem 'factory_girl_rails'

  # Coverage
  gem 'simplecov', require: false

  # Integration tests
  gem 'capybara', require: false
  gem 'launchy', require: false # Used to simplify debugging of Capybara tests
  gem 'poltergeist', require: false
  gem 'minitest-rails-capybara', require: false

  # Stubbing and mocking
  gem 'mocha'
  gem 'webmock'
  gem 'vcr', require: false

  # Better reporters
  gem 'minitest-reporters'

  # Automatic test metadata collection
  gem 'minitest-ci', github: 'circleci/minitest-ci'

  # Make after_commit callbacks fire in tests for Rails 3+ with transactional_fixtures = true.
  # this will no longer needed on rails 5.0+
  gem 'test_after_commit'
end

group :tools do
  gem 'ruby-jmeter', require: false
end
