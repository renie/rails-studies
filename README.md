# RAILS Studies

## System dependencies
	- Ruby 2.4.1
	- Postgres 9.5.8


## Configuration
```
git clone [URL]
cd [clone-path]
gem install bundler
bundle install
```

Create an `.env` file with db usename and password.


## Database creation
```
rails db:migrate
```

Production
```
RAILS_ENV=production rails db:setup
```


## Production Build
```
bundle exec rake assets:clobber
bundle exec rake assets:clean
bundle exec rake assets:precompile
```


## Serve
```
rails s
```

Production:
```
RAILS_SERVE_STATIC_FILES=1 rails s -e production
```


## How to run the test suite
```
rails t
```