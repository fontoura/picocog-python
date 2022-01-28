# Overview
A Python implementation of the picocog library (original Java version by Chris Ainsley).

# Basic usage

The API of this library mostly matches its Java counterpart, but using Python naming conventions. The following code sample generates a 'Hello World' program in Python using this library.

```python
from picocog import PicoWriter

writer = PicoWriter()
writer.writeln("""def hello():""")
writer.indent_right()
writer.writeln("""print('Hello World')""")
writer.indent_left()
writer.writeln("")
writer.writeln("""hello()""")

print(writer.to_string())
```
