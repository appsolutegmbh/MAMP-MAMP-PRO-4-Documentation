---
title: MAMP PRO (Windows) Documentation > How Tos > MySQL
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### How to connect to MySQL using Python 

```python
import mysql.connector

config = {
  'user': 'root',
  'password': 'root',
  'host': 'localhost:8889',
  'database': 'inventory',
  'raise_on_warnings': True,
}

link = mysql.connector.connect(**config)
```