# test-manager-library-3145556-page

> **Technical test · ADSO 3145556** — *Manager Library* static public presentation site (T-23).

- Plain HTML + CSS, no build step and no JavaScript.
- **Never calls the API** and shows no member data (data-model §7): it opens straight from the file system.
- Responsive: fluid type, auto-fit grids and a 16px side gutter; checked at phone and desktop widths.
- Page texts are in Spanish because they are user-facing; code and docs are in English.

## Running it

```bash
open index.html            # or any static server
docker build -t ml-page . && docker run -p 8080:80 ml-page   # http://localhost:8080
```

With `infra`, `docker compose up` serves it at http://localhost:8080.
