source "https://rubygems.org"
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby File.read(".ruby-version").strip

# All runtime config comes from the UNIX environment
# but we use dotenv to store that in files for
# development and testing
gem "dotenv-rails", groups: [:development, :test]

# Brakeman analyzes our code for security vulnerabilities
gem "brakeman"

# bundler-audit checks our dependencies for vulnerabilities
gem "bundler-audit"

# lograge changes Rails' logging to a more
# traditional one-line-per-event format
gem "lograge"

# Ruby < 3.0 included rexml by default, but now
# it's a separate gem that is required for running tests
gem "rexml"

# Bundle edge Rails instead: gem "rails", github: "rails/rails", branch: "main"
gem "rails", "~> 7.0.4"

# The modern asset pipeline for Rails [https://github.com/rails/propshaft]
gem "propshaft"

# Use postgresql as the database for Active Record
gem "pg", "~> 1.1"

# Use the Puma web server [https://github.com/puma/puma]
gem "puma", "~> 6.0"

# Bundle and transpile JavaScript [https://github.com/rails/jsbundling-rails]
gem "jsbundling-rails"

# Hotwire's SPA-like page accelerator [https://turbo.hotwired.dev]
gem "turbo-rails"

# Hotwire's modest JavaScript framework [https://stimulus.hotwired.dev]
gem "stimulus-rails"

# Bundle and process CSS [https://github.com/rails/cssbundling-rails]
gem "cssbundling-rails"

# Build JSON APIs with ease [https://github.com/rails/jbuilder]
gem "jbuilder"

# Use hiredis adapter for better performance than the "redis" gem
gem "hiredis", "~> 0.6.3"

# Use Redis adapter to run Action Cable in production
gem "redis", "~> 5.0"

# Use Kredis to get higher-level data types in Redis [https://github.com/rails/kredis]
# gem "kredis"

# Use Active Model has_secure_password [https://guides.rubyonrails.org/active_model_basics.html#securepassword]
# gem "bcrypt", "~> 3.1.7"

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem "tzinfo-data", platforms: %i[mingw mswin x64_mingw jruby]

# Reduces boot times through caching; required in config/boot.rb
gem "bootsnap", require: false

# Use Active Storage variants [https://guides.rubyonrails.org/active_storage_overview.html#transforming-images]
# gem "image_processing", "~> 1.2"

group :development, :test do
  # See https://guides.rubyonrails.org/debugging_rails_applications.html#debugging-with-the-debug-gem
  gem "debug", platforms: %i[mri mingw x64_mingw]

  gem "standard", require: false
  gem "rubocop", require: false
  gem "rubocop-rails", "2.17.0", require: false
  gem "rubocop-performance", require: false
  gem "rubocop-rspec", "2.14.1", require: false

  gem "rspec-rails", "~> 6.0", ">= 6.0.1"
  gem "factory_bot_rails", "~> 6.2"
  gem "shoulda-matchers", "~> 5.2"
  gem "rspec-html-matchers", "~> 0.10.0"
  gem "database_cleaner-active_record", "~> 2.0", ">= 2.0.1"
  gem "faker", "~> 3.0"
end

group :development do
  # Use console on exceptions pages [https://github.com/rails/web-console]
  gem "web-console"

  # Add speed badges [https://github.com/MiniProfiler/rack-mini-profiler]
  gem "rack-mini-profiler"

  # Speed up commands on slow machines / big apps [https://github.com/rails/spring]
  # gem "spring"
end

group :test do
  gem "rspec_junit_formatter", "~> 0.6.0"
  gem "capybara", "~> 3.38"
  gem "selenium-webdriver", "~> 4.6", ">= 4.6.1"
  gem "webdrivers", "~> 5.2"
  gem "webmock", "~> 3.18", ">= 3.18.1"
end
