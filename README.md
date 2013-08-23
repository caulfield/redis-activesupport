# Redis stores for ActiveSupport

__`redis-activesupport`__ provides a cache for __ActiveSupport__. See the main [redis-store readme](https://github.com/jodosha/redis-store) for general guidelines.

## Installation

```ruby
# Gemfile
gem 'redis-activesupport'
```

### Usage

If you are using redis-store with Rails, consider using the [redis-rails gem](https://github.com/jodosha/redis-store/tree/master/redis-rails) instead. For standalone usage:

```ruby
ActiveSupport::Cache.lookup_store :redis_store # { ... optional configuration ... }
```

## Running tests

```shell
gem install bundler
git clone git://github.com/jodosha/redis-activesupport.git
cd redis-activesupport
bundle install
bundle exec rake
```

If you are on **Snow Leopard** you have to run `env ARCHFLAGS="-arch x86_64" bundle exec rake`

## Copyright

(c) 2009 - 2013 Luca Guidi - [http://lucaguidi.com](http://lucaguidi.com), released under the MIT license
