require 'puppet'
require 'rake'
require 'rspec/core/rake_task'
require 'puppet-lint/tasks/puppet-lint'

PuppetLint.configuration.send("disable_80chars")
PuppetLint.configuration.log_format = "%{path}:%{linenumber}:%{check}:%{KIND}:%{message}"

desc "Run rspec-puppet tests for modules"
RSpec::Core::RakeTask.new(:spec) do |t|
  t.pattern = 'spec/*_spec.rb'
  t.rspec_opts = "--color --format documentation"
end

desc "Run rspec-puppet tests for manifests and modules"
task :default => [:spec]
