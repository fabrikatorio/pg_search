# frozen_string_literal: true

source "https://rubygems.org"

gemspec

gem "pg", ">= 0.21.0", platform: :ruby
gem "activerecord-jdbcpostgresql-adapter", ">= 1.3.1", platform: :jruby

if ENV["ACTIVE_RECORD_BRANCH"]
  gem "activerecord", git: "https://github.com/rails/rails.git", branch: ENV.fetch("ACTIVE_RECORD_BRANCH", nil)
  gem "arel", git: "https://github.com/rails/arel.git" if ENV.fetch("ACTIVE_RECORD_BRANCH", nil) == "master"
end

gem "activerecord", ENV.fetch("ACTIVE_RECORD_VERSION", nil) if ENV["ACTIVE_RECORD_VERSION"]

gem "pry"
gem "rake"
gem "rspec"
gem "rubocop"
gem "rubocop-performance"
gem "rubocop-rails"
gem "rubocop-rake"
gem "rubocop-rspec"
gem "simplecov"
gem "simplecov-lcov"
gem "standard", ">= 1.23.0"
gem "undercover"
gem "warning"
gem "with_model"
