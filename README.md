# Automerge-Convex Quickstart

This is an example [local-first](https://www.inkandswitch.com/local-first) app
using [Automerge](https://automerge.org) and [Convex](https://www.convex.dev).

It demonstrates:

- Modeling data as Automerge `Document`s
- Managing Documents with an Automerge `Repo`:
  - Storing Documents in a client-side IndexedDb
  - Synchronizing Documents with Convex
- Working with Automerge in React:
  - Using a `RepoContext` to expose a repo to UI components
  - Reading & updating documents with the `useDocument` hook

## Installation

Clone the project, install its dependencies, and run `yarn dev` to start the local dev server.

```bash
$ git clone https://github.com/ianmacartney/automerge-convex-quickstart.git
# Cloning into automerge-repo-quickstart...
$ cd automerge-convex-quickstart
$ yarn
# Installing project dependencies...
$ yarn dev
# Starting Vite dev server...
```

Navigate to http://localhost:5173 to see the app running.

You'll notice the URL change to append a hash with an Automerge document ID, e.g.:

`http://localhost:5173/#automerge:8SEjaEBFDZr5n4HzGQ312TWfhoq`

Open the same URL (including the document ID) in another tab or another browser to see each client's changes synchronize with all other active clients.
