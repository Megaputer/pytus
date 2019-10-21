# pytus
yet another tus (resumable file upload protocol) client in python

# Install
```shell
pip install pytus
```

# Usage

The following example uploads a file in single call.

```python
import pytus

FILE_PATH = 'example.bin'
TUS_ENDPOINT = 'https://upload.example.com/files/'

tus = pytus.Client(TUS_ENDPOINT)
with open(FILE_PATH, 'rb') as f:
    tus.upload(f)
```
