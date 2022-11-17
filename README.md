# README

demo_engine gem: https://github.com/hemangini-g-simformsolutions/demoEngine.git

**Steps followed to use gem demo_engine with this application**

gem 'demo_engine', git:'https://github.com/hemangini-g-simformsolutions/demoEngine.git', branch:'main'

bundle install

bin/rails demo_engine:install:migrations

bin/rails db:migrate

add this line in app/assets/config/manifest.js 

//= link demo_engine/application.css

add this line in routes.rb file

mount DemoEngine::Engine => "/demo_engine"

rails s

Go to http://localhost:3000/demo_engine