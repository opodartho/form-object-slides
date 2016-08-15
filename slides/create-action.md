##  Create Action

```ruby

class AlbumController < ApplicationController
  ...
  def create
    @album = Album.create!(album_params)
    #render
  end
  ...
  private

  def album_params
    params.require(:album).permit(:title, :description)
  end
  ...
end
```
