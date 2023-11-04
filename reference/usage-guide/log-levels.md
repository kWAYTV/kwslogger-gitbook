# 💎 Log Levels



{% hint style="info" %}
This assumes you've already created a logger instance called _logger_.
{% endhint %}

## Filter your logs with built-in log levels

Filter out your logs with the built in log levels, anything above the level you set on the logger instace won't be logged nor written to the file.

```
debug (0) --> info (1) --> welcome (2) --> success (3) --> warning (4) --> error (5) --> input (6) --> ratelimit (7) --> sleep (8) --> any (9)
```

Example:

<pre class="language-python"><code class="lang-python"><strong>from kwslogger import Logger
</strong>
# Create a logger instance
logger = Logger(log_level="WARNING", log_to_file=True, log_file_name="mylogs", log_file_mode="a")

print(logger.can_log("INFO")) # --> True because it's below warning level. Would log and write to the file.
print(logger.can_log("RATELIMIT")) # --> False because it's above the warning level. Wouldn't log nor write to the file.
</code></pre>
