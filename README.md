# UTC Simple Log

Simple log with UTC timer.

* Python 3.6 or higher
* Default option
* Both console and File
* Singleton logger

## Quick start
```shell script
$ pip install utc-simple-log
```
```python
"""
example.py
"""
from sslog.logger import SimpleLogger

# Default parameter
# file: './logs/log.txt'
# maxBytes: 2000000 (2Mb) 
# backupCount: 5
logger = SimpleLogger()

logger.setLevel(logging.DEBUG)

logger.debug('hello world!')
logger.info('This is a simple log.')
logger.warning('Quick start')
logger.error('It print to console and')
logger.critical('files("./logs/log.txt")')
logger.fatal('fatal and critical')
```

### Console and File
```bash
2021-03-03T05:54:51, [   DEBUG] [logger.py:_tests,L:147]: Debugging message  
2021-03-03T05:54:51, [    INFO] [logger.py:_tests,L:148]: Info message  
2021-03-03T05:54:51, [ WARNING] [logger.py:_tests,L:149]: Warning message  
2021-03-03T05:54:51, [   ERROR] [logger.py:_tests,L:150]: Error message  
2021-03-03T05:54:51, [CRITICAL] [logger.py:_tests,L:151]: Critical message  
2021-03-03T05:54:51, [CRITICAL] [logger.py:_tests,L:151]: FATAL message
```
