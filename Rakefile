require 'rubygems'
require 'bundler'
require 'rake/testtask'

Bundler::GemHelper.install_tasks

task :test do |test|
  Rake::TestTask.new(:test) do |t|
    t.libs << 'lib' << 'test'
    t.test_files = FileList['test/**/*.rb']
    t.verbose = true
  end
end

task :default => [:build]
