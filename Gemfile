source "http://rubygems.org"

if ENV.key?('PUPPET_VERSION')
  puppetversion = "= #{ENV['PUPPET_VERSION']}"
else
  puppetversion = ['~> 2.7']
end

gem "rake"
gem "puppet", puppetversion
gem "puppet-lint"
gem "rspec-puppet", "0.1.4"
gem "puppetlabs_spec_helper"
