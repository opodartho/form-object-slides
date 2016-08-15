##  prepopulate

```ruby

class AlbumForm < Reform::Form
  ...
  def prepopulate!
    self.title = "Let it shine."
  end
end
```
