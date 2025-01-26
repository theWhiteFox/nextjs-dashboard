## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.`

Node.js 18.18.0 or later installed. Download here [nodejs](https://nodejs.org/en)

This project is using [https://pnpm.io/](https://pnpm.io/)

`npm install -g pnpm`

`pnpm dev`

You can use clsx to conditionally apply the classes [clsx](https://www.npmjs.com/package/clsx)
The `status.tsx` and `pagination.tsx` components use `clsx` to conditionally apply class names.

**why use CSS modules?** 
CSS Modules create unique class names for each component, so you don't have to worry about style collisions.

**Read**
[https://vercel.com/blog/how-core-web-vitals-affect-seo](https://vercel.com/blog/how-core-web-vitals-affect-seo)

Next.js automatically optimizes fonts in the application when you use the next/font module. It downloads font files at build time and hosts them with your other static assets. This means when a user visits your application, there are no additional network requests for fonts which would impact performance.

Next.js downloads font files at build time and hosts them with your other static assets. This means when a user visits your application, there are no additional network requests for fonts which would impact performance.

Images without dimensions and web fonts are common causes of layout shift due to the browser having to download additional resources.

## Routing
### Nested routing

Next.js uses file-system routing where folders are used to create nested routes. Each folder represents a route segment that maps to a URL segment.

By having a special name for page files, Next.js allows you to [colocation](https://nextjs.org/docs/app/building-your-application/routing#colocation) UI components, test files, and other related code with your routes. Only the content inside the page file will be publicly accessible. For example, the /ui and /lib folders are colocated inside the /app folder along with your routes.

Next.js automatically prefetches the code for the linked route in the background. By the time the user clicks the link, the code for the destination page will already be loaded in the background, and this is what makes the page transition near-instant!

[how-routing-and-navigation-works](https://nextjs.org/docs/app/building-your-application/routing/linking-and-navigating#how-routing-and-navigation-works)


One benefit of using layouts in Next.js is that on navigation, only the page components update while the layout won't re-render. This is called [partial rendering](https://nextjs.org/docs/app/building-your-application/routing/linking-and-navigating#4-partial-rendering) which preserves client-side React state in the layout when transitioning between pages.

**Why use layouts?**
That's right, the layout file is the best way to create a shared layout that all pages in your application can use.

[Vercel storage vercel-postgres sdk](https://vercel.com/docs/storage/vercel-postgres/sdk)

That's right, you should not query your database directly when fetching data on the client as this would expose your database secrets.

Server components allow you fetch data directly from your database.

SQL allows you to write targeted queries to fetch and manipulate specific data.

## When might you want to use a waterfall pattern?
To satisfy a condition before making the next request. For example, you might want to fetch a user's ID and profile information first. Once you have the ID, you might then proceed to fetch their list of friends.

to replace the waterfall pattern use 
[MDN Promise all](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/all)

[Nextjs learn static and dynamic rendering](https://nextjs.org/learn/dashboard-app/static-and-dynamic-rendering)

Why might static rendering not be a good fit for a dashboard app?

Because the application will not reflect the latest data changes. When your data updates, you want to show the latest changes in your dashboard. Static Rendering is not a good fit for this use case.

