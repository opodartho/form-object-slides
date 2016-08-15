##  rails populate

```ruby
class Album < ActiveRecord::Base
  before_create :convert_money_to_cents
  attr_accessor :price
  ...
  def convert_money_to_cents
    self.price_in_cents = price.to_i * 100
  end
end
```
