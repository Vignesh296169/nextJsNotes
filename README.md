# nextJsNotes
* Code splitting with React.lazy and Suspense
  - you load only the parts you need right now. When you need other parts, you load them later.
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

* Link
 - react native provides Link component help to navigate between pages
