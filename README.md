
<!--
**betterA/betterA** is a āØ _special_ āØ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- š­ Iām currently working on ...
- š± Iām currently learning ...
- šÆ Iām looking to collaborate on ...
- š¤ Iām looking for help with ...
- š¬ Ask me about ...
- š« How to reach me: ...
- š Pronouns: ...
- ā” Fun fact: ...
-->
### betterA āļø ![](https://views.whatilearened.today/views/github/betterA/betterA.svg)


```python
from __future__ import annotations

import json
from dataclasses import asdict, dataclass


@dataclass
class BetterA:
    languages: tuple[str, ...] = ("Python", "JS", "Go")
    databases: tuple[str, ...] = ("SQLite", "MySQL", "MongoDB", "Redis")
    misc     : tuple[str, ...] = ("Docker", "Celery", "RabbitMQ", )
    ongoing  : tuple[str, ...] = ("Django", "DRF", "Flask", "grpc")

    def jsonify(self) -> str:
        return json.dumps(asdict(self), indent=4)


bettera = BetterA()
print(bettera.jsonify())
```

