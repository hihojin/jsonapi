# jsonapi

# Description
Extends python's json library to serialize and deserialize complex and range objects. Includes pytest.

# Installation 
## Development Mode
In the root directory, run the following: pip install -e .

# Sample Code
import json

class BetterEncoder(json.JSONEncoder):
    ...

class BetterDecoder(json.JSONDecoder):
    ...

def dumps(data, cls=BetterEncoder):
    return json.dumps(data, cls=cls)

def loads(data, cls=BetterDecoder):
    return json.loads(data, cls=cls)
