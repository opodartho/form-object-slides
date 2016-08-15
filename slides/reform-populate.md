##  reform populate

```ruby
class AlbumForm < Reform::Form
  property :title
  property :description
  property :price,
    type: Types::Form::Integer,
    populator: ->(fragment:, **) { fragment * 100 }

  validates :title, presence: true
  validates :description, presence: true
end
```
