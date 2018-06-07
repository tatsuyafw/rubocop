# frozen_string_literal: true

source 'https://rubygems.org'

gemspec

gem 'bump', require: false
gem 'pry'
# pry-byebug requires MRI 2.2.0 or higher.
gem 'pry-byebug' if RUBY_ENGINE == 'ruby' && RUBY_VERSION >= '2.2.0'
gem 'rake', '~> 12.0'
gem 'rspec', '~> 3.7'
gem 'rubocop-rspec', '~> 1.26.0'
gem 'simplecov', '~> 0.10'
gem 'test-queue'
gem 'yard', '~> 0.9'

group :test do
  gem 'codeclimate-test-reporter', '~> 1.0', require: false
  gem 'safe_yaml', require: false
  gem 'webmock', require: false
end

local_gemfile = 'Gemfile.local'
eval_gemfile local_gemfile if File.exist?(local_gemfile)
