
begin
  require 'jasmine'
  load 'jasmine/tasks/jasmine.rake'
rescue LoadError
  task :jasmine do
    abort "Jasmine is not available. In order to run jasmine, you must: (sudo) gem install jasmine"
  end
end

desc "Package extension into .zip"
task :package do
  system('zip -r -x=extension/coffeescripts/* extension.zip extension')
end