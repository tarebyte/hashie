source 'http://rubygems.org'

gemspec

group :development do
  gem 'pry'
  gem 'pry-stack_explorer', platforms: [:ruby_19, :ruby_20, :ruby_21]
  gem 'rubocop', '0.34.2'
  gem 'guard', '~> 2.6.1'
  gem 'guard-rspec', '~> 4.3.1', require: false
end

group :test do
  # ActiveSupport required to test compatibility with ActiveSupport Core Extensions.
  if RUBY_VERSION >= '2.2.2'
    gem 'activesupport', '~> 5.x', require: false
    gem 'activemodel', '~> 5.x', require: false
  else
    gem 'activesupport', '~> 4.x', require: false
  end
  gem 'dry-types', require: false
  gem 'codeclimate-test-reporter', require: false
  gem 'rspec-core', '~> 3.1.7'
  gem 'danger-changelog', '~> 0.1.0', require: false
end
