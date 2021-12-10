
<!--
**betterA/betterA** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
### betterA ✈️ ![](https://views.whatilearened.today/views/github/betterA/betterA.svg)


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

