# Integración PMA — Documentación de API

Documentación técnica del endpoint `APIPmaValidateToken` para pruebas internas con Postman.

## Contenido

| Archivo | Descripción |
|---|---|
| `index.html` | Documentación completa — abrir directo en el navegador |
| `image.png` | Captura Postman: colección INTEGRACIÓN PMA |
| `image copy.png` | Captura Postman: respuesta exitosa (Success: true) |
| `image copy 2.png` | Captura Postman: TOKEN_ALREADY_USED |
| `image copy 3.png` | Captura Postman: TOKEN_NOT_FOUND |

## Cómo usar

1. Clonar o descargar el repositorio
2. Abrir `index.html` en cualquier navegador
3. No requiere servidor ni dependencias — funciona como archivo estático

> Las imágenes deben estar en la misma carpeta que `index.html` para que la galería funcione correctamente.

## Endpoint documentado

```
POST http://192.168.0.32/CertificacionFEProduccion/rest/APIPmaValidateToken
```

### Respuestas posibles

| ErrorCode | Success | Descripción |
|---|---|---|
| *(vacío)* | `true` | Token válido |
| `TOKEN_NOT_FOUND` | `false` | Token no existe |
| `TOKEN_ALREADY_USED` | `false` | Token ya fue usado |
| `TOKEN_EXPIRED` | `false` | Token vencido |

## Stack

- HTML + CSS puro (sin dependencias externas en runtime)
- Fuentes: [Fraunces](https://fonts.google.com/specimen/Fraunces) · [IBM Plex Mono](https://fonts.google.com/specimen/IBM+Plex+Mono) · [Outfit](https://fonts.google.com/specimen/Outfit) via Google Fonts
- Compatible con todos los navegadores modernos
