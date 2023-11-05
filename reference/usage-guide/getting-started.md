# ⭐ Getting Started



## Importing and creating Instance

First, you need to import and create an instance of the Logger, here's how to do so:

```python
from kwslogger import Logger

# Create a logger instance
logger = Logger(log_level="ANY", log_to_file=True, log_file_name="mylogs", log_file_mode="a")
```

{% swagger method="options" path="" baseUrl="Logger" summary="Logger class parameters" %}
{% swagger-description %}
Here are the parameters you can set for each logger instance.
{% endswagger-description %}

{% swagger-parameter in="body" name="log_level" type="String" %}
The log level to use for logging messages
{% endswagger-parameter %}

{% swagger-parameter in="body" name="log_to_file" type="Boolean" %}
Whether to log messages to a file or not
{% endswagger-parameter %}

{% swagger-parameter in="body" name="log_file_name" type="String" %}
The name of the log file to use
{% endswagger-parameter %}

{% swagger-parameter in="body" name="log_file_mode" type="String" %}
The mode to use when opening the log file
{% endswagger-parameter %}

{% swagger-parameter in="body" name="timestamps_timezone" type="String" %}
The pyqtz timezone to use for timestamps.
{% endswagger-parameter %}
{% endswagger %}
