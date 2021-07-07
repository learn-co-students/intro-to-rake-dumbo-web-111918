task :environment do
  require_relative './config/environment'
end

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


namespace :sports do
  desc 'Nba association'
  task :nba do
    puts "NBA is the best sport organization"
  end
  desc "Mlb Association"
  task :mlb do
    puts "MLB is good too"
  end
end


namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end
  desc 'seed the database with some dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end
end

desc 'drop into the pry console'
task :console => :environment do
  Pry.start
end
