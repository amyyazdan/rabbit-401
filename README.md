# Rabbit 401

Lightweight In Memory Key Value Database For Python 3+

---

## How to use?

Install package from [PyPi](https://pypi.org/project/rabbit-401/) using `pip` command in terminal:

```plaintext
pip install rabbit-401
```

Then, in your program:

```python
from rabbit_401 import Rabbit401

r401 = Rabbit401()

# Insert
r401.insertItem("Value") # If you don't give your key, It will generate a unique 24 length key (using bson.objectid.ObjectId)
r401.insertItem("Another Value", "key1")

# Get
r401.getItem("key1") # It's safe and it will return None if key is not valid.

# Delete
r401.insertItem("key1") # It's safe and it will return None if key is not valid.
```