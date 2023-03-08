## Prerequsites

Must have a GitHub OAuth app .
GitHub app's client ID and client secret must be present in a `.env` file in the project root.

`AUTH_SECRET` must be present in the `.env` with a random, 32-character string. You can generate one with `openssl rand -hex 32`.

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.
