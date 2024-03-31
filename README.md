# rot-kbd

A highly insecure encryption scheme based on rot13 and keyboard layouts

```pycon
>>> from rot_kbd import *

>>> rot_wertyq('qwerty')
'wertyu'
>>> rot_yqwert(rot_wertyq('qwerty'))
'qwerty'

>>> rot_wertyq('wasd')
'esdf'
>>> rot_yqwert(rot_wertyq('wasd'))
'wasd'
```
