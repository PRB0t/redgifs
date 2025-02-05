<h1 align="center"> <code>redgifs</code> </h1>

<div align="center">
    <a href="https://pypi.org/project/redgifs">
        <img src="https://img.shields.io/pypi/v/redgifs.svg" alt="pypi">
    </a>
    <a href="https://github.com/scrazzz/redgifs/actions/workflows/test.yml">
        <img src="https://github.com/scrazzz/redgifs/actions/workflows/test.yml/badge.svg" alt="pytest">
    </a>
</div>

<p align="center"> Async and Sync Python Wrapper for the Redgifs API. </p>

```
⚠ This project is still in development.
```

### Installation
```
pip install -U redgifs
```

`redgifs` works on Python versions 3.7 and above.

### Quickstart
Synchronous usage
```py
import redgifs

api = redgifs.API()
response = api.search('3D')
print(response)
api.close()
```

Asynchronous usage
```py
import asyncio
from redgifs.aio import API

async def main():
    api = API()
    response = await api.search('3D')
    print(response)
    await api.close()

loop = asyncio.get_event_loop()
loop.run_until_complete(main())
```

More examples can be found in the examples directory.

### Documentation
https://redgifs.readthedocs.io
