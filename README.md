# PyTokenize
Tokenize C++/C code in Python using LibClang.

# Usage
Include tokenizer.py in your current working directory:

"""Python
from tokenizer import Tokenizer

tok = Tokenizer("../path/to/code.cpp")

entire_token_stream = tok.full_tokenize()
tokens_per_function = tok.split_functions(False) # Set to True if we only one methods attached to classes
"""

**Note:** You may need to update the path to the libclang library in tokenizer.py. Obviously, you also need libclang installed.

# Testing
To run my breif test code:

python tokenizer.py <relative path to C/C++ file>

This will use the library's split_functions functionality to print out a list of functions and their tokenizations.
