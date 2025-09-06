\# API Reference



import PyCliffordMCP

import inspect



with open("\_docs/api\_reference.md", "w") as f:

&nbsp;   f.write("# API Reference\\n\\n")

&nbsp;   for name, obj in inspect.getmembers(PyCliffordMCP):

&nbsp;       if inspect.isclass(obj) or inspect.isfunction(obj):

&nbsp;           f.write(f"## {name}\\n\\n")

&nbsp;           doc = inspect.getdoc(obj)

&nbsp;           f.write(doc + "\\n\\n" if doc else "No docstring provided.\\n\\n")



