namespace :greeting do
desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hola to the terminal'
  task :hola do
    puts "hola de Rake!"
  end
end

desc 'Opening console?'
  task :console do
    puts "I exist"
  end

  task :environment do
    require_relative './config/environment'
  end

namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'seed data base with dummy data'
  task :seed => :environment do
    require_relative './db/seeds.rb'
  end
end
