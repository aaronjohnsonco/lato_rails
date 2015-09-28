# LatoRails

This is a gem to add the Lato font to your rails application using the asset pipeline. 

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'lato_rails'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install lato_rails

## Usage

The Lato font is installed and accessible using the following when declaring your classes in your view templates:

```ruby
latohairline  # font-family: "latohairline"
latohairline_italic  # font_family: "latohairline_italic"

latolight  # font-family: "latolight"
latolight_italic  # font-family; "latolight_italic" 

latoregular  # font-family: "latoregular"
latoregular_italic  # font-family: "latoregular_italic"

latobold  # font-family: "latobold"
latobold_italic  # font-family: "latobold_italic"

latoblack  # font-family: "latoblack"
latoblack_italic  # font_family: "latoblack_italic"
```

In the app/assets/stylesheets/application.css file add the following:

```ruby
*= require 'lato'
```

or you can change your application.css file to application.scss and add the following:

```ruby
@import 'lato';
```
In development you will need to add the following to the config/environments/development.rb file:

```ruby
config.assets.precompile << /\.(?:svg|eot|woff|ttf)\z/
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/lato_rails.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

