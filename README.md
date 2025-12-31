# Signalgrid Python Client
[![PyPI version](https://badge.fury.io/py/signalgrid.svg)](https://pypi.org/project/signalgrid/)
[![Python versions](https://img.shields.io/pypi/pyversions/signalgrid)](https://pypi.org/project/signalgrid/)

Official Python client for the Signalgrid push-notification API.

## Installation

```bash
pip install signalgrid
```
## Example
```python
from signalgrid.client import Client

client = Client("YOUR_CLIENT_KEY")

response = client.send({
    "channel": "CHANNEL_TOKEN",
    "type": "info",
    "title": "Hello from Python",
    "body": "This message was sent from a test project.",
    "critical": False
})

print(response)
```
## Response
```
{"ruuid":"bc0e212110067ff2995abff087a4a58c8d843ae9","text":"OK","code":"200","node":"dp03","time":"440ms","remaining":"99917"}
```
