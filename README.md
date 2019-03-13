# Capistrano::LoadVariables

Load configuration variables from YAML file.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'capistrano-load_variables'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install capistrano-load_variables

## Usage

Add this line to your Capfile after ```require "capistrano/setup"```.

```ruby
require 'capistrano/load_variables'
```

Put ```cap_variables.yml``` in ```config``` directory.

```yaml
staging:
  url: http://staging.example.com/
  port: 3000
production:
  url: http://www.example.com/
  port: 80
```

In staging and production stage, ```url``` and ```port``` will be set.
