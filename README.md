# ActAsTimeAsBoolean

_Add time_as_boolean feature to your ruby classes_

## Installation

```shell
gem install act_as_time_as_boolean
```

Or in your Gemfile:

```ruby
gem 'act_as_time_as_boolean'
```

## Usage

```ruby
class Item
  include ActAsTimeAsBoolean

  attr_accessor :archived_at

  time_as_boolean :archived
end

item = Item.new

p item.archived?
#=> false

item.archived = Time.now
p item.archived?
#=> true
```

## Contributing

1. Fork repository
2. Create a branch following a [successfull branching model](http://nvie.com/posts/a-successful-git-branching-model/)
3. Write your feature/fix
4. Write tests
5. Pull request

## Licence

Released under the MIT License. See the [LICENSE](https://github.com/caedes/act_as_time_as_boolean/blob/master/LICENSE.md) file for further details.
