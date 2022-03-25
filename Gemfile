# frozen_string_literal: true

source 'https://rubygems.org'

# as framework
gem 'rails', '~> 7.0'
# as asset pipeline
gem 'sprockets-rails'
# as application server
gem 'puma'

# for appdata redirections (https -> http)
gem 'open_uri_redirections'

# for stylesheets
gem 'sassc-rails'

# as javascript asset compressor
gem 'terser'

# for translations
gem 'fast_gettext', '>= 0.7.0'
gem 'gettext_i18n_rails', '>= 0.4.3'

# rails-i18n provides translations for ActiveRecord
# validation error messages
gem 'rails-i18n'

# Generate html based on markdown in views
gem 'redcarpet', '~> 3.5.1'

# for logging
gem 'lograge'

gem 'dalli'
gem 'hashie'
gem 'mini_magick'
gem 'minitest'
gem 'nokogiri'
gem 'xmlhash', '>= 1.2.2'

gem 'matrix'
gem 'prometheus_exporter'
gem 'puma_worker_killer'

# FIXME: for selenium-webdriver, rexml isn't in the default set of Ruby 3.1 anymore
# see https://github.com/SeleniumHQ/selenium/commit/526fd9d0de60a53746ffa982feab985fed09a278
gem 'rexml'

# HTTP client library for OBS Client
gem 'faraday'
gem 'faraday_middleware'
gem 'multi_xml'

# needed to collect translatable strings
# not needed at production
group :development do
  # no need to load the gem via require
  # we only need the rake tasks
  gem 'gettext', '>= 1.9.3', require: false
end

group :test do
  gem 'capybara'
  gem 'faker'
  gem 'geckodriver-bin', '~> 0.28.0'
  gem 'rubocop'
  gem 'rubocop-minitest'
  gem 'rubocop-performance'
  gem 'rubocop-rails'
  gem 'selenium-webdriver'
  gem 'vcr'
  gem 'webmock'
  gem 'simplecov', require: false
end

group :development, :test do
  gem 'byebug'
end
