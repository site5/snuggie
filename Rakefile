$:.unshift 'lib'

require 'rake/testtask'

Rake::TestTask.new do |test|
  test.libs << "test"
  test.test_files = FileList['test/**/*_test.rb']
end

task :default => :test

desc "Open an irb session preloaded with this library"
task :console do
  sh "irb -rubygems -r ./lib/snuggie.rb -I ./lib"
end
