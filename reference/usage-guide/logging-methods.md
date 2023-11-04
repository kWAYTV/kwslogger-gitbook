# 🛣 Logging Methods



{% hint style="info" %}
This assumes you've already created a logger instance called _logger_.
{% endhint %}

## Log messages

Example:

```python
from kwslogger import Logger

# Create a logger instance
logger = Logger()

# Clear the console
logger.clear()

# Log a message
logger.welcome("I'm a welcome message!")
logger.info("I'm an info message!")
logger.debug("I'm a debug message!")
logger.success("I'm a success message!")
logger.warning("I'm a warning!")
logger.error("I'm an error!")
logger.input("I'm an input message!")
logger.ratelimit("I'm a rate limit message!")
```
