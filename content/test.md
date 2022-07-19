+++
title = "Coding Patterns to Avoid Leaking Secrets"
date = 2022-07-15

[taxonomies]
tags = ["python", "rust", "security"]
+++

# The Problem

So hear is the deal, I love logs. We all love logs, but we can get a bit over zealous at times with what we log. Especially as security professionals we tend to want everything and it is our default advice, _just in case_. :smile:

Consider we have a Python class that represents some user information. To keep it brief, we will hold the `name` and `social_security_number` of a user:

```python
class UserInfo:

  def __init__(self, name: str, social_security_number: str):
    self.name = name
    self.social_security_number = social_security_number
```

# The Imperfect Solution

# Leak Detection
