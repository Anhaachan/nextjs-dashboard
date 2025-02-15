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
- Move data fetches down to the components that need it is good practice when working with Suspense and data fetching
- adding skeleton to page for loading

# Chapter 10
Partial Prerendering

- Partial Prerendering is an experimental feature introduced in Next.js 14. **PPR is only available with the Next.js canary releases (next@canary),**
- Partial Prerendering - is a new rendering model that allows you to combine the benefits of static and dynamic rendering in the same routes.


> Previuos chapter's recap will go here.
---------

> Ah, shit here we go again.

# Chapter 11
Adding Search and Pagination

- ## Why use URL search params?
 This pattern may be new if you're used to doing it with client side state.

There are a couple of benefits of implementing search with URL params:

- Bookmarkable and shareable URLs: Since the search parameters are in the URL, users can bookmark the current state of the application, including their search queries and filters, for future reference or sharing.
- Server-side rendering: URL parameters can be directly consumed on the server to render the initial state, making it easier to handle server rendering.
- Analytics and tracking: Having search queries and filters directly in the URL makes it easier to track user behavior without requiring additional client-side logic.


- handled search and pagination with URL search parameters instead of client state.
-  fetched data on the server.
- useRouter router hook for smoother, client-side transitions.

# Chapter 12
Mutating data

- CRUD
- React server actions
- FormData object
- revalidatePath API

# Chapter 13
> ah shit here we go again.
