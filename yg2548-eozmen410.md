# Project Proposal


## Background and Motivation
There is a hole in deserealization/validation libraries for Python. There exist [libraries](https://json-schema.org/) that allow you to deserealize data but often involve coming up with tedious schemas to define it. Deserealization should also be extensible. You don't want to be restricted to only JSON or YMAL.

## volga

**volga is a framework for *de*serealizing Python data structures**

volga will allow you to *flow* your data into any format that you'd like.

```python3
  import volga-json
  
  @Deserealize
  def class User():
    name: Annotated<str, volga-json.exclude('yefri')>
    age: int
  
  
  # ...
  
  deserealized = volga-json.from_string(json_string)
```

## Future Enhancements
