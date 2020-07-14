---
title: Flask+Request实现web接口
date: 2020/7/14
tags:
  - Web
  - Python
categories: python
---

废话不多说,代码!

web.py:
```python
from flask import  Flask
app = Flask(__name__)
import tokengenerator

@app.route('/')
def index():
    return '<h1>Welcome To NGEdit Active Code Port!</h1>'

@app.route('/token')
def index():
  return tokengenerator.token()

if __name__ == '__main__':
    app.run(port=80)
```

tokengenerator.py:
```Python
import time
import random


lsa = list("12aAbBcCdDeEfFgGhHiIjJkK9lLm78MnNoO56pPqQrLsStTuUvV34wWxXyYzZ")
def token:
    p = random.choice(lsa)
    p1 = random.choice(lsa)
    p2 = random.choice(lsa)
    p3 = random.choice(lsa)
    p4 = random.choice(lsa)
    p5 = random.choice(lsa)
    p6 = random.choice(lsa)
    p7 = random.choice(lsa)
    p8 = random.choice(lsa)
    p9 = random.choice(lsa)
    p10 = random.choice(lsa)
    p11 = random.choice(lsa)
    p12 = random.choice(lsa)
    p13 = random.choice(lsa)
    p14 = random.choice(lsa)



    hole = p+p1+p2+p3+p4+p5+p6+p7+p8+p9+p10+p11+p12+p13+p14
    return hole
```

crawl.py:
```python
import request

response = request.get("http://localhost:80/token")
print(response.text)
```

(介绍以后再做,睡觉去了)
