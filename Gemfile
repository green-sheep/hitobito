# encoding: utf-8

#  Copyright (c) 2012-2014, Jungwacht Blauring Schweiz. This file is part of
#  hitobito and licensed under the Affero General Public License version 3
#  or later. See the COPYING file at the top-level directory or at
#  https://github.com/hitobito/hitobito.

source 'https://rubygems.org'

gem 'rails', '4.2.4'

gem 'activerecord-session_store'
gem 'airbrake'
gem 'awesome_nested_set'
gem 'bcrypt-ruby'
gem 'cancancan'
gem 'carrierwave'
gem 'cmess'
gem 'country_select'
gem 'daemons'
gem 'dalli'
gem 'delayed_job_active_record'
gem 'devise'
gem 'draper'
gem 'faker'
gem 'globalize'
gem 'haml'
gem 'http_accept_language'
gem 'magiclabs-userstamp', require: 'userstamp'
gem 'mini_magick'
gem 'mysql2', '0.3.15' # 0.3.16 fails sphinx specs on jenkins
gem 'nested_form'
gem 'oat'
gem 'paper_trail'
gem 'paranoia'
gem 'customized_piwik_analytics', '~> 1.0.0'
gem 'prawn', '< 2.0' # 2.0 requires ruby 2.0
gem 'prawn-table'
gem 'protective'
gem 'rack'
gem 'rails_autolink'
gem 'config'
gem 'rails-i18n'
gem 'seed-fu'
gem 'simpleidn'
gem 'thinking-sphinx'
gem 'validates_by_schema'
gem 'validates_timeliness'
gem 'wagons'

# load after others because of active record inherited alias chain.
gem 'kaminari'

# Gems used only for assets
gem 'bootstrap-sass', '~> 2.3'
gem 'bootstrap-wysihtml5-rails', '~> 0.3.1.24'
gem 'chosen-rails'
gem 'coffee-rails'
gem 'compass'
gem 'compass-rails'
gem 'jquery-rails'
gem 'jquery-ui-rails'
gem 'sass-rails'
gem 'therubyracer', platforms: :ruby
gem 'uglifier'

group :development, :test do
  gem 'binding_of_caller'
  gem 'rspec-rails'
  gem 'sqlite3'
  gem 'codez-tarantula', require: 'tarantula-rails3'
  gem 'pry-rails'
  gem 'pry-debugger', platforms: :ruby_19
  # gem 'pry-byebug', platforms: [:ruby_20, :ruby_21]
end

group :development do
  gem 'bullet'
  gem 'quiet_assets'
  gem 'redcarpet'
  gem 'request_profiler'
end

group :test do
  gem 'capybara'
  gem 'database_cleaner'
  gem 'fabrication'
  gem 'headless'
  gem 'launchy'
  gem 'rspec-its'
  gem 'rspec-collection_matchers'
  gem 'selenium-webdriver'
end

group :console do
  gem 'awesome_print'
  gem 'hirb'
  gem 'mailcatcher'
  gem 'pry-doc'
  gem 'pry-remote'
  gem 'pry-stack_explorer'
  gem 'rdoc-tags'
  gem 'spring-commands-rspec'
  gem 'wirble'
end

group :metrics do
  gem 'annotate'
  gem 'brakeman'
  gem 'ci_reporter_rspec'
  gem 'rails-erd'
  gem 'rubocop'
  gem 'rubocop-checkstyle_formatter'
  gem 'ruby-prof'
  gem 'simplecov-rcov'
end

# Include the wagon gems you want attached in Wagonfile.
# Do not check Wagonfile into source control.
#
# To create a Wagonfile suitable for development, run 'rake wagon:file'
wagonfile = File.expand_path('../Wagonfile', __FILE__)
eval(File.read(wagonfile)) if File.exist?(wagonfile)
