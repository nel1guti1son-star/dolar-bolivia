# Dólar Bolivia (PWA)

App móvil en español con tipo de cambio **oficial BCB** y **paralelo P2P**.

## Archivos
- `index.html` — UI + lógica
- `manifest.webmanifest` — instalar / Add to Home Screen
- `sw.js` — caché offline de la app y última respuesta de APIs
- `icons/` — iconos 192/512

## Fuentes
- Oficial: `GET https://apibcb.cucu.bo/api/v1/tc/oficial`
- Paralelo: `GET https://paralelo.bo/api/v1/rate` (CC-BY 4.0)

## Servir local
```bash
cd /workspace/dolar-bolivia && python3 -m http.server 8765
```

## Publicar (necesita cuenta)
Cualquiera de estos, autenticado:

```bash
# GitHub Pages (recomendado si tienes gh auth)
# Netlify: netlify deploy --dir=/workspace/dolar-bolivia --prod
# Vercel:  vercel /workspace/dolar-bolivia --prod
# Surge:   surge /workspace/dolar-bolivia tu-nombre.surge.sh
```
