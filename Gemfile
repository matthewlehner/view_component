# frozen_string_literal: true

source "https://rubygems.org"
gemspec

rails_version = (ENV["RAILS_VERSION"] || "~> 7.0.0").to_s

gem "capybara", "~> 3"
gem "apparition"
gem "rails", (rails_version == "main") ? {git: "https://github.com/rails/rails", ref: "main"} : rails_version

gem "rspec-rails", "~> 5"

group :test do
  gem "cuprite", "~> 0.8"
  gem "puma", "~> 5"

  gem "selenium-webdriver", "~> 4"
end

if RUBY_VERSION >= "3.1"
  gem "net-imap", require: false
  gem "net-pop", require: false
  gem "net-smtp", require: false
end
