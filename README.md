# EqualsTrue

## General tools for python 
Tasker example

```python
from datetime import timedelta
from equalstrue.tasker import Tasker
from winsound import Beep
tasker = Tasker()

@tasker.register(interval=timedelta(seconds=2))
def beeps(*args,**kwargs):
    Beep(1000,1000)

tasker.run()
```


