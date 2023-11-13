# 🍫 Progress Bars



Create progress bars with ease.

```python
import time
from kwslogger import Logger

logger = Logger()

for i in (logger.progress_bar(range(100), desc="Progress Bar", unit="items", unit_scale=True, unit_divisor=100, miniters=1, mininterval=0.1, maxinterval=1, dynamic_ncols=True, smoothing=0.3, bar_format="{l_bar}{bar}| {n_fmt}/{total_fmt} [{elapsed}<{remaining}]", leave=False)):
    time.sleep(0.1)
```

You can add as many arguments and customizations as the [tqdm ](https://github.com/tqdm/tqdm)library supports.
