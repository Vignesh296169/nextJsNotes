# nextJsNotes
* Code splitting with React.lazy and Suspense
  - you load only the parts you need right now. When you need other parts, you load them later.
  - SEO: Much better SEO performance since the content is pre-rendered and easily crawlable by search engines.
* Server Components
   - Your friend (the server) builds some parts, and you (your computer) build other parts, and together you create the whole castle (your app) more easily and quickly!
* Pnpm
   - Project A needs lodash -> Stores lodash in a central place.
   - Project B needs lodash -> Links to the same lodash stored for Project A.
* Setup Project
  - npx create-next-app@latest nextjs-dashboard --example "https://github.com/vercel/next-learn/tree/main/dashboard/starter-example" --use-pnpm
 
* Inbuild routing system no need to install third party routing like react ,, because that is library not a framework
  - app folder -> page.js is a initiall file which renders first in browser
  - app folder -> about folder -> page.js

* Link setup 
  - react native provides Link component help to navigate between pages.
  - why-because when we use anchor tag the pages will re-renders so we use link tag in react and next js.
  - In Next.js, useRouter is a React hook that provides access to the routing functionalities within your client-side components. It's particularly useful for 
    programmatically navigating between routes or accessing information about the current route.(Important have to import from the next/navigation not from 
    next/router) -> only working in client components("use client").
* Components .
   - Initailly a next js  create file into server component (server side jobs)
   - when you need to use server or client component (https://nextjs.org/docs/app/building-your-application/rendering/composition-patterns)
* Dynamic routes.
  - Web Development: In the context of URLs, as mentioned before, a slug is a part of a web address that identifies a specific page in a readable way.
  - App folder -> Items folder ->[slug] folder ->page.js==Localhost:3000/Items/id
  - Use Params props in function and get the string query
  - item folder->[...slug] floder=> multi dynamic routes you will get ({params})=>params.slug  []
* Route Handler
  - route.js file holding the api related stuff
  - new Response() this will return the value , you can see the api request on network tap
  - if you want return the array json Response.json() remove the new key word
  - (thunder client) is library for vs code. set up the post man locally
* Query params on route
  -in url -> localhost:800/item ? type ="finish" this query you can get in api function -> req -> req.nextUrl.searchParam.get()
  -post api -> req.json() -> here you can access the post body values.
* components
  - you can create the component out side of app folder
  - db related stuff like model and connection -> utils should outside of app route and folder.
  - create mongo db model as singler noun collection will create pural form post-> posts
  - by default you can not use .env property in client component
  - in front of .env property you need to just add NEXT_PUBLIC_API_TOKEN, SO with this client compoent access the .env key
