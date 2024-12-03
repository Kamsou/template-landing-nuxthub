# Starter landing page

A minimal [Nuxt](https://nuxt.com) starter deployed on the Edge using [NuxtHub](https://hub.nuxt.com).

https://aucreno.pages.dev/

<a href="https://aucreno.pages.dev/">
<img src="/public/capture.png" alt="Capture" />
</a>

## Features

- Server-Side rendering on Cloudflare Workers
- ESLint setup
- Ready to add a database, blob and KV storage
- One click deploy on 275+ locations for free
- Tailwind

## Setup

Make sure to install the dependencies with [pnpm](https://pnpm.io/installation#using-corepack):

```bash
yarn
```

You can update the main text displayed by creating a `.env`:

```bash
NUXT_PUBLIC_HELLO_TEXT="Hello my world!"
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
yarn dev
```

## Production

Build the application for production:

```bash
yarn build
```

## Deploy


Deploy the application on the Edge with [NuxtHub](https://hub.nuxt.com) on your Cloudflare account:

```bash
npx nuxthub deploy
```

Then checkout your server logs, analaytics and more in the [NuxtHub Admin](https://admin.hub.nuxt.com).

You can also deploy using [Cloudflare Pages CI](https://hub.nuxt.com/docs/getting-started/deploy#cloudflare-pages-ci).
