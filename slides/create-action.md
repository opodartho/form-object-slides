##  Create Action

```ruby

class PostController < ApplicationController
  ...
  def create
    @post = Post.create!(post_params)
    #render
  end
  ...
  private

  def post_params
    params.require(:post).permit(:name, :description)
  end
  ...
end
```
