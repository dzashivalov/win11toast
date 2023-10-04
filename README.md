[![Python](https://img.shields.io/pypi/pyversions/win11toast.svg)](https://badge.fury.io/py/win11toast)
[![PyPI](https://badge.fury.io/py/win11toast.svg)](https://badge.fury.io/py/win11toast)

# win11toast
Toast notifications for Windows 10 and 11 based on [WinRT](https://docs.microsoft.com/en-us/windows/apps/design/shell/tiles-and-notifications/adaptive-interactive-toasts)
This is fork of [win11toast](https://github.com/GitHub30/win11toast) project.
It has been modified for work inputs with dictionary.

## Dictionary Usage

```python
from win11toast import toast

inputs = {'id0': ["title0", "placeHolder0"], 'id1': ["title1", "placeHolder1"], 'id2': ["title2", "placeHolder2"]}
toast("Inputs with dictionary", "Type anything", inputs=inputs, button='Send')
# {'arguments': 'http:Send', 'user_input': {'id0': 'value0', 'id2': 'value2', 'id1': 'value1'}}
```

![image](https://github.com/dzashivalov/win11toast/blob/main/inputs_screenshot.png)

https://docs.microsoft.com/en-us/uwp/schemas/tiles/toastschema/element-input
