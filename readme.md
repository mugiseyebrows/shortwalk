# shortwalk

`os.walk` that can go no deeper than you want it to, and can jump over obstacles.

## Install

```
pip install shortwalk
```

## Use

```python
from shortwalk import walk

for root, dirs, files in walk(path, maxdepth=2, skip=['.git', '*.egg-info']):
    for file in files:
        do_stuff_with(file)
```