# GAP — Portal de Tasas

Sitio estático que muestra tasas en tiempo real (referencia: VES), histórico simulado y calculadoras (conversor y brecha).

Características
- Obtiene tasas desde exchangerate.host usando VES como referencia (se calcula USD/VES y EUR/VES).
- Trata USDT como equivalente a USD (USDT ≈ USD).
- Caching local en localStorage con fallback.
- Polling cada 60 segundos.
- GitHub Actions workflow para desplegar en GitHub Pages.

Ejecutar localmente
1. Crea una carpeta y guarda `index.html` dentro.
2. Ejecuta un servidor estático:

Con Python 3:
```bash
python -m http.server 8000
# abre http://localhost:8000
.
