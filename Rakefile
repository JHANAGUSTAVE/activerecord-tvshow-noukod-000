# require_relative 'config/environment.rb'

# namespace :db do

#   desc "Migrate the db"
#   task :migrate do
#     connection_details = YAML::load(File.open('config/database.yml'))
#     ActiveRecord::Base.establish_connection(connection_details)
#     ActiveRecord::Migrator.migrate("db/migrate/")
#   end

#   desc "drop and recreate the db"
#   task :reset => [:drop, :migrate]

#   desc "drop the db"
#   task :drop do
#     connection_details = YAML::load(File.open('config/database.yml'))
#     File.delete(connection_details.fetch('database')) if File.exist?(connection_details.fetch('database'))
#   end
# end



ENV["SINATRA_ENV"] ||= "development"

require_relative './config/environment'
require 'sinatra/activerecord/rake'

# Type `rake -T` on your command line to see the available rake tasks.

task :console do
  Pry.start
end

