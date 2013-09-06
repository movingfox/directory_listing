require "bundler/gem_tasks"
require 'rake/testtask'
require 'yard'

##
# Run the test application

task :run do
  `ruby test/test_directory_listing_app.rb -o 0.0.0.0`
end

##
# Generate yard docs

YARD::Rake::YardocTask.new do |t|
  t.files = ['lib/**/*.rb']
end

##
# Run tests

Rake::TestTask.new do |t|
  t.libs << 'test'
end
