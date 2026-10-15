# HMLabs Gaming Website

The documentation site for HMLabs-Gaming, published at
[gaming.hmlabs.eu](https://gaming.hmlabs.eu). It is built with [Astro](https://astro.build)
and [Starlight](https://starlight.astro.build).

The site currently documents:

- Modpacks
- Resource packs
- Mods
- Plugins

## Requirements

- Node.js LTS
- npm

## Development

Install dependencies and start the development server from this directory:

```bash
npm install
npm run dev
```

The site is available at [http://localhost:4321](http://localhost:4321). Astro watches the
source files and reloads the page as you work.

## Commands

| Command           | Description                        |
| ----------------- | ---------------------------------- |
| `npm run dev`     | Start the development server       |
| `npm run build`   | Build the static site into `dist/` |
| `npm run preview` | Serve the production build locally |
| `npm run start`   | Alias for the development server   |
| `npm run astro`   | Run the Astro CLI                  |

The production build is the project's automated validation check. There is currently no
separate lint or test script.

## Project structure

```text
public/                  Files served directly, including browser scripts
src/assets/              Project artwork and badges
src/components/          Custom Astro and Starlight components
src/content/docs/        Markdown and MDX documentation pages
src/content.config.ts    Content collection configuration
astro.config.mjs         Site metadata, integrations, and sidebar
vercel.json              Legacy project redirects
```

Documentation pages are created below `src/content/docs/`. Their paths become site URLs;
for example, `src/content/docs/projects/modpacks/hmt-pack/installation.mdx` is available at
`/projects/modpacks/hmt-pack/installation/`. Add pages to the sidebar in
`astro.config.mjs` when they should appear in site navigation.

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) for writing guidance, navigation updates, asset
conventions, validation steps, and pull request expectations. For a local production check,
run:

```bash
npm run build
```

The site does not require environment variables. Do not commit secrets, local environment
files, or generated `dist/` output.

## Deployment

Astro generates a static site in `dist/`. The canonical URL is configured in
`astro.config.mjs`, and `vercel.json` preserves redirects from older project URLs to their
current documentation pages. Deployment is handled by the hosting configuration for the
site.

## Links

- [Live site](https://gaming.hmlabs.eu)
- [GitHub organization](https://github.com/HMLabs-Gaming)
- [Discord community](https://discord.gg/EHU4YMaHGT)
- [Modrinth organization](https://modrinth.com/organization/9zYhowm8)
- [CurseForge projects](https://www.curseforge.com/members/henrymmey/projects)

## License

This repository uses a multi-license model. Source code, configuration, and scripts are
licensed under [MIT](./LICENSE); written documentation is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/);
and logos, icons, project artwork, and other branding assets are All Rights Reserved. See
[LICENSE](./LICENSE) for the complete terms.
