  # Figures et images
 
  {% for picture in book.pictures_list %}
    1. [{{ picture.list_caption }}]({{ picture.backlink }})
  {% endfor %}
  
  