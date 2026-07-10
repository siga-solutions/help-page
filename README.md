# help-page

Página de ayuda de SIGA (Centro de Ayuda), embebida en el frontend vía el
módulo **Ayuda** (`ayuda_url` en `application_settings`).

## Contenido

- `index.html` — guía de usuario en español (módulos reales de la app)
- `styles.css` — estilos del layout colapsable
- `images/` — capturas e iconos de referencia

## Vista local

```bash
open index.html
# o cualquier servidor estático, p.ej.:
python3 -m http.server 8080
```

## Actualización

Al cambiar pantallas o flujos en el frontend, revise y ajuste esta guía.
Reemplace o amplíe `images/` cuando haya pantallas nuevas relevantes
(Instrumentos, Transacciones, Perfiles, Informe Anual).

## Enlace en la aplicación

El frontend carga la URL configurada en Supabase:

```text
application_settings.key = 'ayuda_url'
```

Apunte ese valor a la URL pública donde se publique este sitio estático.
