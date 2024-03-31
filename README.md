# rot-kbd

A highly insecure encryption scheme based on rot13 and keyboard layouts

Use as a Python module

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

Or on the command line

```console
$ echo 'qwerty' | python -mrot_kbd
wertyu
$ echo 'qwerty' | python -mrot_kbd | python -mrot_kbd --rotation rot_yqwert
qwerty
```
