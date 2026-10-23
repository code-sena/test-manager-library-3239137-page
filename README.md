# test-manager-library-3239137-page

Sitio público de presentación de **Manager Library**. Cuenta qué es el sistema y
qué reglas lo rigen; **no habla con la API**.

## Cómo verlo

Se abre con doble clic en `index.html`: son dos archivos estáticos, sin build y
sin dependencias.

```bash
# o, si se prefiere servirlo:
python -m http.server 4173
```

## Qué contiene

| Archivo | Qué es |
|---|---|
| `index.html` | La página: qué hace el sistema, las reglas de negocio y para quién es |
| `styles.css` | Estilos propios, sin framework |

## Decisiones

- **Sin framework ni build.** Es una página de presentación: un `index.html` y
  un `styles.css` se abren en cualquier parte y no caducan.
- **Correcto en móvil y escritorio.** Rejilla fluida con `auto-fit`, y las
  reglas pasan de dos columnas a una por debajo de 680 px.
- **Sin datos reales.** No pide nada a la API, así que se puede publicar sin
  exponer el sistema.
