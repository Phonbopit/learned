## How to enable logger on test environment (RSpec)?

Edit a file : `config/environment/test.rb`

```ruby
config.logger = Logger.new(STDOUT)

# config.log_level = :debug, :info, :error
```
