# Justipy

This package allows you to draw justified text to images.

Installation:
```pip install justipy```

Usage example:

```python
from PIL import Image
from Justipy.Justipy import Justipy

longtext = "Lorem ipsum vehicula himenaeos turpis odio sollicitudin quis amet suspendisse nisl, libero taciti ante interdum sollicitudin vestibulum felis mi hac, egestas fames luctus turpis imperdiet consectetur est gravida sem. malesuada maecenas vivamus consectetur donec diam sapien, in erat curae phasellus potenti, sed primis velit sem cursus. molestie ultrices tempus arcu viverra eleifend primis malesuada convallis ante accumsan, pulvinar conubia mollis at pellentesque consectetur ut dapibus sagittis integer nam, tempus orci elementum curabitur id rhoncus tempus velit elit. mollis vestibulum curabitur laoreet augue faucibus nullam a amet justo lorem, varius placerat magna pulvinar aptent quis porttitor metus lacus, diam etiam auctor nulla sagittis metus urna phasellus vitae."

im = Image.new('RGB', (1000, 500))
jpy = Justipy(im,
              longtext,
              tl_corner = [100, 75],
              max_width = 800,
              fontsize = 24,
              line_space = 32,
              paragraph_spaces = 8,
              font = 'calibri.ttf',
              fontcolor = (255,255,255)).getImage()

jpy.show()
```
