source "https://rubygems.org"

git_source(:github) { |repo| "https://github.com/#{repo}.git" }

gemspec

if ENV['CUCUMBER_RUBY_CORE']
  gem 'cucumber-core', path: ENV['CUCUMBER_RUBY_CORE']
elsif !ENV['CUCUMBER_USE_RELEASED_GEMS']
  gem 'cucumber-core', github: 'cucumber/cucumber-ruby-core'
end

if ENV['CUCUMBER_RUBY']
  gem 'cucumber', path: ENV['CUCUMBER_RUBY']
elsif !ENV['CUCUMBER_USE_RELEASED_GEMS']
  gem 'cucumber', github: 'cucumber/cucumber-ruby'
end

gem 'aruba', git: 'https://github.com/cucumber/aruba.git', branch: 'allow-new-cucumbers'
