source 'https://rubygems.org'

branch = ENV.fetch('SOLIDUS_BRANCH', 'master')
gem 'solidus', github: 'solidusio/solidus', branch: branch
gem 'solidus_auth_devise'

if branch == 'master' || branch >= "v2.3"
  gem 'rails', '~> 5.1.0' # hack for broken bundler dependency resolution
elsif branch >= "v2.0"
  gem 'rails', '~> 5.0.0' # hack for broken bundler dependency resolution
else
  gem "rails", '~> 4.2.0' # hack for broken bundler dependency resolution
end

gem 'pg'
gem 'mysql2'

gemspec
