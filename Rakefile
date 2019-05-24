# desc 'outputs hello to the terminal'
# task :hello do
#   puts "hello from Rake!"
# end


namespace :greeting do
  desc 'gives greeting in 2 languages'
  task :hello do
    puts "hello from Rake!"
  end

  task :hola do
    puts "hola de Rake!"
  end

end

namespace :db do
  desc 'migrate changes to your database'
  task :environment do
    require_relative './config/environment'
  end
  task :migrate => :environment do
    Student.create_table
  end
end

namespace :db do
  desc 'seed database with some dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end
end

task :console do
  Pry.start
end
