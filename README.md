# Installing Node

Install node through the Node Version Manager (`nvm`).

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
nvm install node
```

# create-svelte

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm create svelte@latest

# create a new project in my-app
npm create svelte@latest my-app
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.

## Storybook

Adding storybook with svelte/typescript support requiers the the cutting edge
version of storybook (v7.0.0-beta.31). There is also a bug where you'll have to remove node_modules and redownload everything. Strange. Hopefully they fix that in version 7. In the meantime:

```bash
rm -rf node_modules
rm package-lock.json
npm install
npx sb@next init
```

Anyways, after installing storybook, run storybook with:

```bash
$ npm run storybook
```