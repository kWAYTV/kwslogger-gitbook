# 💤 Sleep & Spinners





## Animated Sleeps

Our library provides you with a fancy way of sleeping in the terminal, check this out:

```python
from kwslogger import Logger

# Create a logger instance
logger = Logger()

logger.sleep("Waiting for 1 second...", 1)
```

***

## Run functions with spinner

Run functions while you showing the spinner with an optional timer

```python
import time
from kwslogger import Logger

# Create a logger instance
logger = Logger()

def test_func(number1, number2):
    answer = number1 + number2
    time.sleep(3)
    return answer

result = logger.run_with_spinner(test_func, "Calculating...", True, 1, 1)
print(str(result) + " (Func returned)")
```
