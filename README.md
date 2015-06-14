# PyTokenize
Tokenize C++/C code in Python using LibClang.

# Usage
Include tokenizer.py in your current working directory:

```python
from tokenizer import Tokenizer

tok = Tokenizer("../path/to/code.cpp")

entire_token_stream = tok.full_tokenize()

# Set argument to True if we only want methods attached to classes
tokens_per_function = tok.split_functions(False)
```

**Note:** You may need to update the path to the libclang library in tokenizer.py. Obviously, you also need libclang installed.

# Testing
To run my brief test code in a terminal:

> python tokenizer.py ../relative/path/to/code/file.cpp

This will use the library's split_functions functionality to print out a list of functions and their tokenizations.

# Further Notes
This library has been customized for use in cheating detection applications. It should be pretty simple to un-customize it.
