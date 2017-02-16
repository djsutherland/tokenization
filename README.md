Some Python utilities to make [MapTool](http://www.rptools.net/toolbox/maptool/) tokens for Pathfinder NPCs/monsters/etc.

Currently pretty specific to our particular campaign properties / etc.

# tokens.py

Interface to make MapTool token files.

Example usage:

```
import tokens
import requests

r = requests.get('http://vignette3.wikia.nocookie.net/forgottenrealms/images/3/36/Monster_Manual_5e_-_Ogre_-_p237.jpg')
image = tokens.Asset('ogre', 'jpg', r.content)
t = Token(image=image, name='Ogre', )
```
