[![Gem Version](https://badge.fury.io/rb/cleanrpc.svg)](https://badge.fury.io/rb/cleanrpc)

# Cleanrpc


## Installation

Add this line to your application's Gemfile:

```ruby
gem 'cleanrpc'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install cleanrpc

## Usage


```
$ ./bin/console
irb(main):001:0> rpc = Cleanrpc::Rpc.new("http://aUser:aPassword@localhost:8332")
=> #<Cleanrpc::Rpc:0x0000000103787bf8 @uri=#<URI::HTTP http://aUser:aPassword@localhost:8332>>
irb(main):002:0> rpc.getblockcount
=> 816336
irb(main):003:0>
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and the created tag, and push the `.gem` file to [rubygems.org](https://rubygems.org).

```
rake build                    # Build cleanrpc-0.0.1.gem i...
rake build:checksum           # Generate SHA512 checksum i...
rake clean                    # Remove any temporary products
rake clobber                  # Remove any generated files
rake install                  # Build and install cleanrpc...
rake install:local            # Build and install cleanrpc...
rake release[remote]          # Create tag v0.0.1 and buil...
rake rubocop                  # Run RuboCop
rake rubocop:autocorrect      # Autocorrect RuboCop offens...
rake rubocop:autocorrect_all  # Autocorrect RuboCop offens...
rake spec                     # Run RSpec code examples
```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/BrantaOps/cleanrpc.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
