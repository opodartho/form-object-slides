##  reform new action

```ruby
def new
  @form = PostForm.new(Post.new)
end
```
