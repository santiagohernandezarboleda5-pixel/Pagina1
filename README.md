# ServirPRO – clon de 3 páginas

Páginas incluidas (copiadas sin cambios del proyecto original, rama `prod`):

| Ruta | Archivo |
|---|---|
| `/` | `src/pages/index.astro` |
| `/seguros-vehiculo` | `src/pages/seguros-vehiculo.astro` |
| `/compra-cartera-vehiculos` | `src/pages/compra-cartera-vehiculos.astro` |

`src/pages/api/send-email.ts` se mantiene porque el formulario de `/compra-cartera-vehiculos` lo usa.

## Uso

```sh
cp .env.example .env   # y completar RESEND_API_KEY
pnpm install
pnpm dev               # http://localhost:4321
pnpm build
```

## Dónde están los colores

- Tokens de marca: `src/styles/global.css` (bloque `@theme`).
- Colores sueltos (hex / `bg-[#...]`) dentro de los componentes en `src/components/`.
