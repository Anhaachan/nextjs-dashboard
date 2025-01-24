# Chapter 1
Getting started

- `pnpm` i don't user personally use this but i nextjs recommended this for efficient.
```bash
npm install -g pnpm
```

- then use this command for creating new project using blueprint example.
```bash
npx create-next-app@latest nextjs-dashboard --example "https://github.com/vercel/next-learn/tree/main/dashboard/starter-example" --use-pnpm
```

- run project
```bash
pnpm dev
```
-------
# Chapter 2
CSS Styling

- Global styles

## Tailwind
- `create-next-app` will ask you use tailwind if click `yes` the it will automatically configure settings.

---------
# Chapter 3
Optimizing Fonts and Images

- Cumulative Layout Shift 

- add custom fonts. But if using `next/font` it will be more useful for optimization

## `<Image` component

- Preventing layout shift automatically when images are loading.
- Resizing images to avoid shipping large images to devices with a smaller viewport.
- Lazy loading images by default (images load as they enter the viewport).
- Serving images in modern formats, like WebP and AVIF, when the browser supports it.

--------
# Chapter 4
Creating Layouts and Pages

- understanding nested routing

- understand layout

One benefit of using layouts in Next.js is that on navigation, only the page components update while the layout **won't re-render.**

> purpose of the layout file is to share UI across multiple pages