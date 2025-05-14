## 🧱 Estructura básica de un workflow

Un archivo de workflow en GitHub Actions (por ejemplo, .github/workflows/ci.yml) se divide así:
```yaml
name: Nombre del workflow

on:            # ← EVENTO (cuándo se ejecuta)
  push:
    branches: [main]

jobs:          # ← JOBS (qué tareas hacer)
  build:       # ← Un job
    runs-on: ubuntu-latest
    steps:     # ← STEPS (pasos dentro del job)
      - name: Paso 1
        run: echo "Hola mundo"
```
