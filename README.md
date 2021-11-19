## Trying to reproduce a problem

The `component` directory contains a svelte-kit shareable component, along with `component/src/routes/index.svelte` that 
exercises it.  It's a simple pagination component.

The `app` directory contains a svelte-kit app that uses this shareable component, and it is run from `app/src/routes/index.svelte`.

Both of these apps build in the usual svelte kit way, so to get it all running:

 * cd component
 * npm install
 * npm run build

This packages the svelte component into `component/package`.  To run the app

 * cd app
 * npm install
 * npm run dev

Browse to localhost:3000 to see the paginator component reuses.

## Unable to reproduce the problem

When I did something like this in a larger context, in a mono repo using rushjs, I was unable to use the shared
component in the app.  So I have failed to reproduce it in this smaller repo.  Too bad.

If/when I figure out the root cause in my larger repo, I will amend this repo to contain the issue, so it can be fixed.