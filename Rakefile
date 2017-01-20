#!/usr/bin/env ruby

require 'rake'

task :vagrantfile do
  Dir['**/Vagrantfile'].each { |f| sh "rubocop #{f}" }
end

task :rubyfile do
  Dir['**/*.rb'].each { |f| sh "rubocop #{f}" }
end

task :default => [:vagrantfile, :rubyfile]
