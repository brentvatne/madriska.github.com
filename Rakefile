require 'compass'

namespace :jekyll do
  desc 'Delete generated _site files'
  task :clean do
    system "rm -rf _site"
  end

  desc 'Run the jekyll dev server'
  task :server do
    system "jekyll --server --auto"
  end

  desc 'Clean temporary files and run the server'
  task :compile => [:clean] do
    system "compass:clean"
    system "compass:compile"
    system "jekyll"
  end
end
