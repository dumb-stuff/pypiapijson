# Pypiapijson!
Welcome to pypiapijson documentation! (Reworked)
## Uses
Please read [this](https://warehouse.pypa.io/api-reference/index.html#rate-limiting) for ratelimiting stuff (Not really neccessary here.)
## What's new
I have async module and block module by import module and use 
```py
import pypiapijson
pypiapijson.asyncs # this is async module
pypiapijson # this is module block code :D
```
The usage async module is same as block but await it **NOT** `async with` like
```py
await pypiapijson.asyncs.get("Flask") # ✔ Good way to use async function

async with pypiapijson.asyncs.get("Flask") # ❌ **NOT** Correct way to use it
```
## Script
```py
pypiapijson.get(name : str)
```
This function get the package by the name if it isn't exist it return None
```