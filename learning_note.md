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

--------
# Chapter 5
Navigating between pages

- Automatic code-splitting and prefetching
- using 'Link' component nextjs can route throught the pages. most important is when you use 'Link' in your page then nextjs will prefetches data in the client and show that page instantly.

# Chapter 6
Setting up databases

1. Import project from github in `vercel`.
2. Create Database in vercel using `serverless postgres by **Neon**`
3. Seed database wiht nextjs `Route Handlers`

# Chapter 7
Fetching Data

- Choosing how to fetch data

1. API Layer
- In Next.js, you can create API endpoints using Route Handlers.

2. Database queries
- When you're creating a full-stack application, you'll also need to write logic to interact with your database

3. Using Server Components to fetch data

4. Using SQL
- write database queries using the Vercel Postgres SDK and SQL. 

! Static Rendering

# Chapter 8
Static and Dynamic Rendering

- Simulating a Slow Data Fetch
With dynamic rendering, **application is only as fast as your slowest data fetch.**

# Chapter 9
Streaming

- advantages of streaming is : chunks are rendered in parallel, reducing the overall loadtime.
