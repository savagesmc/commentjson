# commentjson

`commentjson` (Comment JSON) is a Python package that helps you create JSON
files with comments. Its API is very similar to the Python standard library's
[json][json] module.

[json]: http://docs.python.org/2/library/json.html

## Installation

```
pip install commentjson
```

## Basic Usage

```python
>>> import commentjson
>>>
>>> json_string = """{
...     "name": "Vaidik Kapoor", # Person's name
...     "location": "Delhi, India",
...
...     # Section contains info about person's appearance
...     "appearance": {
...         "hair_color": "black",
...         "eyes_color": "black",
...         "height": "6"
...     }
... }"""
>>>
>>> json_loaded = commentjson.loads(json_string)
>>> print json_loaded
{u'appearance': {u'eyes_color': u'black', u'hair_color': u'black', u'height': u'6'}, u'name': u'Vaidik Kapoor', u'location': u'Delhi, India'}
```

## Tests

```
python setup.py test
```
