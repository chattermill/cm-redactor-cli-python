# Chattermill Standalone Data Redaction Tool

### How it works:
The script runs a series of Regular Expressions to remove certain patterns from text. You can customise the list of Regular Expressions to run. You can also use as Python module for more custom workflows.

### Install:
 * Install requirements using `pip install -r requirements.txt`
 * Clone git repo in the right folder: `git clone https://github.com/chattermill/cm-redactor-cli-python.git`

### Run:
To run in the command line:
```
python redact.py "My email is contact@chattermill.io"
=> My email is [redacted]
```
To use as a module:
```
from redact import Redactor
...
redactor = Redactor()
redacted = redactor.apply_rules('My email is contact@chattermill.io')
```

### Credits
Forked from Chattermill
