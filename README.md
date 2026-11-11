# haugestol.com

My personal site: [haugestol.com](https://haugestol.com). It has a project showcase, a CV page, recent GitHub activity and a contact form.

## Stack

- TanStack Start (React, file-based routing, server functions)
- Tailwind CSS, shadcn/Base UI components, Motion, three.js
- Paraglide (inlang) for Norwegian and English
- GitHub GraphQL API for the activity feed and Resend for contact mail
- Docker for deployment

## Run

```sh
pnpm install
pnpm dev      # http://localhost:3000
```

Server features need these environment variables:

| Variable | Used for |
| --- | --- |
| `GITHUB_TOKEN` | Activity section (GitHub GraphQL) |
| `RESEND_API_KEY` | Contact form |

`pnpm screenshots` regenerates the project screenshots in `src/assets/screenshots`.

## Layout

- `src/routes/`: pages (`/`, `/projects`, `/cv`)
- `src/components/sections/`: home page sections
- `src/content/`: project, CV and site copy
- `src/server/`: server functions for GitHub data and the contact form
- `messages/`: translations
