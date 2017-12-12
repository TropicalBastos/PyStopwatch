# PyStopwatch

Easy to use threaded stopwatch for python

###Examples:

```python
import time
from stopwatch import Stopwatch

sw = Stopwatch()
sw.start()
time.sleep(2)
sw.stop()
print(sw.get_time()) #prints 2.0s

sw.reset() #reset anytime after stopping
sw.start() #let's restart the timer
time.sleep(10)
sw.stop()
print(sw.get_time()) #prints 10.0s

# returns the raw floating point number to 3 decimal places (milliseconds)
print(sw.get_time(raw = True))
```