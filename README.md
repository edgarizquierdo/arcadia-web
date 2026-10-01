# Arcadia Global Analytics — nueva web

Prototipo estático listo para revisar y desplegar.

## Abrir en local

Desde Terminal:

```bash
cd Arcadia_Global_Analytics_Web
python3 -m http.server 8080
```

Abrir: http://localhost:8080

## Atlas BioScan

URL demo: `http://localhost:8080/atlas/login.html`

Contraseña demo: `ATLAS-2026`

Atlas no aparece en la navegación pública, no está en `sitemap.xml`, lleva `noindex,nofollow` y está bloqueado en `robots.txt`.

**Importante:** la contraseña JavaScript sirve solamente para revisar la demo. Para que Atlas sea realmente privado en producción, activar autenticación HTTP a nivel de servidor usando uno de estos ejemplos:

- `atlas/_htaccess.example` (Apache)
- `atlas/nginx-location.example.conf` (Nginx)

La autenticación del servidor debe ser la capa real de seguridad.

## SEO incluido

- títulos y metadescripciones diferentes por página
- canonical
- Open Graph básico
- datos estructurados Organization
- sitemap XML
- robots.txt
- arquitectura temática separada para agricultura y software

## Pendientes antes de producción

1. Sustituir/recuperar política de privacidad, cookies, aviso legal y términos actuales.
2. Conectar el formulario a backend, Formspree, Brevo u otro proveedor.
3. Integrar imágenes/capturas reales de viñedo, plataforma y proyectos.
4. Añadir logos de clientes/partners con permiso de uso.
5. Configurar Analytics / Search Console y banner de cookies.
6. Endurecer `/atlas/` con autenticación del servidor.
