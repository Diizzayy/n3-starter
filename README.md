# Nuxt 3 Minimal Starter with ESLint

Look at the [nuxt 3 documentation](https://v3.nuxtjs.org) to learn more.

## Template Changes

- ESLint
- Stub Nuxt Types on install
- Prefer [Volar's Take Over Mode](https://github.com/johnsoncodehk/volar/discussions/471)

## New Project

```sh
npx nuxi init -t diizzayy/n3-starter nuxt-app
```

## Prettier as an ESLint Rule

```sh
# yarn
yarn add -D prettier eslint-plugin-prettier eslint-config-prettier 

# npm
npm install -D prettier eslint-plugin-prettier eslint-config-prettier 

# pnpm
pnpm install -D prettier eslint-plugin-prettier eslint-config-prettier 
```

### Add Prettier Config

Create a file named `.prettierrc` in the root of your project and add the code below.

```json
{
    "semi": false,
    "tabWidth": 2,
    "singleQuote": true,
    "trailingComma": "none"
}
```

### Add `plugin:prettier/recommended` as the **LAST** ESLint extension`

```
{
  "extends": [
    "@nuxtjs/eslint-config-typescript",
    "plugin:prettier/recommended"
  ]
}
```

## Install Dependencies

Make sure to install the dependencies:

```bash
# yarn
yarn install

# npm
npm install

# pnpm
pnpm install --shamefully-hoist
```

## Development Server

Start the development server on http://localhost:3000

```bash
npm run dev
```

## Production

Build the application for production:

```bash
npm run build
```

Locally preview production build:

```bash
npm run preview
```

Checkout the [deployment documentation](https://v3.nuxtjs.org/guide/deploy/presets) for more information.
