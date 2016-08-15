##  reform validation

```ruby
class AlbumForm < Reform::Form
  property :title
  property :description

  validates :title, presence: true
  validates :description, presence: true
end
```
