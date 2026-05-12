# @emreunes/medusa-category-images

Medusa v2 plugin that adds category image management to the Admin category detail page.
This package is a production-ready, reusable plugin adaptation of Medusa's [`category-images` example](https://github.com/medusajs/examples/tree/main/category-images).  
Instead of copying example files manually, you can install this plugin directly to get the same core functionality (admin widget, API routes, workflows, and data model) in a packaged form.

## Features

- Adds an Admin widget to category detail pages
- Upload and manage category images
- Supports thumbnail/image type handling
- Includes API routes and workflows for category image CRUD

## Requirements

- Node.js 20+
- Medusa v2.14.x
- pnpm 11+

## Development

```bash
pnpm install
pnpm medusa plugin:develop
```

## Build

```bash
pnpm medusa plugin:build
```

## Usage in Medusa Project

Install:

```bash
pnpm add @emreunes/medusa-category-images
```

Register plugin in your Medusa config:

```ts
// medusa-config.ts
export default defineConfig({
  plugins: [
    {
      resolve: "@emreunes/medusa-category-images",
      options: {},
    },
  ],
});
```

Then run migrations/build in your Medusa app as usual.

## Notes

- Build warning about `deepMerge` in generated `__admin-extensions__.js` does not block build.
