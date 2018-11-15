# Todos API
 [![license](https://img.shields.io/github/license/mashape/apistatus.svg)]() 
Languages : Ruby, Framework : Rails
Basic API JSON with RSpec (TDD) 

# Pre
    Ruby version 2.5.0 or higher
    Postgresql
    Bundler
    Rails

# Gem
- [Rspec-rails](https://github.com/rspec/rspec-rails) - Testing framework.
- [Factory_bot_rails](https://github.com/thoughtbot/factory_bot_rails) - Perlengkapan uji test.
- [shoulda_matchers](https://github.com/thoughtbot/shoulda-matchers) - Menyediakan Rspec dengan matcher tambahan.
- [database_cleaner](https://github.com/DatabaseCleaner/database_cleaner) - Membersihkan Database setelah melakukan Test.
- [faker](https://github.com/stympy/faker) - Data Dummy untuk Test RSpec.

# Run Local
  
    git clone <url repo> | Clone this repo
    bundle install | Install gem
    rake db:create | Create database
    rake db:migrate | Create migration
    rails server | Running rails server in localhost
    running at http://localhost:3000

# Run Local Rubocop
  
  
    bundle exec rubocop <your_file> [options]
    [options] : Auto Correct = -a
                Rails-intensive = -R
    
# Run Local RSpec
    bundle exec rspec
    Directory RSpec are in Todos-api/spec

# Run Local Manual Test to the API
    GET /todos
    http :3000/todos
    POST /todos
    http POST :3000/todos title=Mozart created_by=1
    PUT /todos/:id
    http PUT :3000/todos/1 title=Beethoven
    DELETE /todos/:id
    http DELETE :3000/todos/1

# Run Local Manual Test to todo items API
    GET /todos/:todo_id/items
    http :3000/todos/2/items
    POST /todos/:todo_id/items
    http POST :3000/todos/2/items name='Listen to 5th Symphony' done=false
    PUT /todos/:todo_id/items/:id
    http PUT :3000/todos/2/items/1 done=true
    DELETE /todos/:todo_id/items/1
    http DELETE :3000/todos/2/items/1

# Author
Refiqi Muhamad Fadila | refyfadhila96@gmail.com