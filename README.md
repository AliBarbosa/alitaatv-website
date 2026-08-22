# Web de AlitaaTV

Página oficial hecha con Astro y Tailwind CSS. Se publica con Cloudflare Workers Static Assets.

## Actualizar contenido

En GitHub abre `src/data/site.ts`. Ahí puedes cambiar la biografía, horario, correo, Twitch y redes. Pulsa **Commit changes** para guardar.

Para cambiar imágenes, abre `public/images/`, elige **Edit** → **Choose file** y conserva estos nombres: `profile.png` (imagen principal), `banner.jpg` (vídeos), `logo-mark.png` (cabecera) y `logo-round.png` (logo circular).

Los botones de clips enlazan hoy a YouTube, TikTok y Twitch. Cuando tengas enlaces de vídeos concretos, puedes pedirme que los inserte. La sección de merchandising está preparada como “Próximamente”.

## Seguridad y despliegue

No subas contraseñas, claves API ni tokens al repositorio. Esta web no necesita secretos. Si en el futuro hicieran falta, añádelos en Cloudflare: **Workers & Pages → tu Worker → Settings → Variables and Secrets**, usando **Encrypt**.

Para publicar desde esta carpeta: `npm run build` y después `npx wrangler deploy`. `wrangler.jsonc` publica la carpeta `dist` como Static Assets.

---

# Astro Starter Kit: Minimal

```sh
npm create astro@latest -- --template minimal
```

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
