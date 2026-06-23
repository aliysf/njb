# PT NJB Company Profile Website

Responsive bilingual construction company profile website for PT NJB, designed as a static site for Vercel.

## Features

- Indonesian and English language switcher with browser persistence
- Mobile-friendly sticky navigation and responsive sections
- Interactive construction service cards, animated counters, portfolio filters, and contact form
- Static build output for Vercel deployment

## Local development

```bash
npm start
```

Preview the production build:

```bash
npm run build
npm run preview
```

## Updating content

Most website copy is managed in `public/app.js` inside the `translations` object. Update the Indonesian (`id`) and English (`en`) sections there when official construction project details or profile content are available.

## Vercel

The repository includes `vercel.json` configured to:

- run `npm run build`
- publish the `dist` directory

Use the Vercel project name `pt-njb` to target the production URL:

```text
https://pt-njb.vercel.app
```

Recommended deployment flow from an authenticated Vercel CLI session:

```bash
npx vercel login
npx vercel link --project pt-njb
npx vercel --prod
```
