# 🆎 Logos



{% hint style="info" %}
This assumes you've already created a logger instance called _logger_.
{% endhint %}

## Create & print a logo

Create logos with just 1 function

```python
from kwslogger import Logger

logger = Logger()

logger.create_logo("Pluto Reportbot")
```

You can use a custom [pyfiglet](https://github.com/pwaller/pyfiglet) font with the following

```python
logger.create_logo("Pluto Reportbot", font = "slant")
```
