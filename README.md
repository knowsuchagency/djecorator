# Djecorator

Djecorator is a Python package that provides a simple and intuitive way to define Django URL routes using decorators, similar to flask.

## Installation

```
pip install djecorator
```

## Usage

The main component of Djecorator is the Route class. You can create an instance of this class and use it as a decorator to define your routes.

Here is a basic example:

```python
from django.shortcuts import render
from djecorator import Route

route = Route()

@route("/")
def index(request):
    return render(request, "index.html")
```

Accessing routes
You can access the defined routes using the patterns and names properties of the Route instance.

patterns
The patterns property returns a list of Django URL patterns.

The names property returns a dictionary where the keys are the route names and the values are the corresponding paths.

Contributing
Contributions are welcome! Please feel free to submit a pull request.

License
Djecorator is released under the MIT License.
