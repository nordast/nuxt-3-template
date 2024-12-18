## Setup

Make sure to install the dependencies:

```bash
npm install
```

### Environment Variable Setup

Copy the variables from .env.example file and create new file called .env.

### Development Server

Start the development server on [http://localhost:3000](http://localhost:3000):

```bash
npm run dev
```


###
## Self installation
###

#### Install Latest Nuxt Project [#](https://nuxt.com/docs/getting-started/installation#new-project)

```bash
npx nuxi@latest init <project-name>
```

#### Install Nuxt Color Mode:

```bash
npx nuxi module add color-mode
```

#### Shadcn Setup [#](https://www.shadcn-vue.com/docs/installation/nuxt.html)

```bash
npm install -D typescript

npx nuxi@latest module add @nuxtjs/tailwindcss

npx nuxi@latest module add shadcn-nuxt
```

Update the nuxt.config.ts as following:

 ```javascript
export default defineNuxtConfig({
  modules: ['@nuxtjs/tailwindcss', 'shadcn-nuxt'],
  shadcn: {
    prefix: '',
    componentDir: './components/ui'
  }
})
```


 ```bash
#Run the CLI:
npx shadcn-vue@latest init

#Install button component:
npx shadcn-vue@latest add button
 ```


#### VueUse [#](https://vueuse.org/guide/#nuxt)

```bash
npx nuxi@latest module add vueuse
```

#### ESLint and Prettier [#](https://eslint.nuxt.com/packages/module#quick-setup)

```bash
npx nuxi module add eslint
npm i -D eslint prettier eslint-config-prettier eslint-plugin-prettier
```

Add to the eslint.config.mjs:
```javascript
import withNuxt from "./.nuxt/eslint.config.mjs";

import eslintPluginPrettierRecommended from "eslint-plugin-prettier/recommended";

export default withNuxt(eslintPluginPrettierRecommended);
```

Add the below to lint commands to your package.json script section:
```json
{
    "scripts": {
        "lint": "eslint .",
        "lint:fix": "eslint . --fix",
        "format": "prettier --write \"{components,pages,plugins,middleware,layouts,composables,assets}/**/*.{js,jsx,ts,tsx,vue,html,css,scss,json,md}\""
    }
}
```

#### Fonts [#](https://fonts.nuxt.com/get-started/installation#automatic-installation)

```bash
npx nuxi@latest module add fonts
```

#### Icons [#](https://nuxt.com/modules/icon#setup-%EF%B8%8F)

```bash
npx nuxi@latest module add icon
```

#### SEO [#](https://nuxtseo.com/docs/nuxt-seo/getting-started/installation)

```bash
npx nuxi@latest module add @nuxtjs/seo
```

#### Third-Party Scripts [#](https://scripts.nuxt.com/docs/getting-started/installation)

```bash
npx nuxi@latest module add scripts
```

#### Auto-animate [#](https://nuxt.com/modules/auto-animate#installation)

```bash
npm install @formkit/auto-animate
```

#### Nuxt Cloudinary  [#](https://cloudinary.nuxtjs.org/getting-started#installation)

```bash
npm install @nuxtjs/cloudinary
```

Update the nuxt.config.ts as following:

 ```javascript
export default defineNuxtConfig({
   modules: [
   "@nuxtjs/cloudinary"
   ],
})
```

Add env variables in the .env.

```
NUXT_PUBLIC_CLOUDINARY_CLOUD_NAME=""
NUXT_PUBLIC_UPLOAD_PRESET=
NUXT_CLOUDINARY_API_KEY=""
NUXT_CLOUDINARY_API_SECRET=""
```

###
## 
###


#### Nuxt Auth Utils  [#](https://github.com/atinux/nuxt-auth-utils)

```bash
npx nuxi@latest module add auth-utils
```
Add a NUXT_SESSION_PASSWORD env variable with at least 32 characters in the .env.
```
NUXT_SESSION_PASSWORD=""
```

#### Prisma

```bash
npm install -D prisma @prisma/client
```

Some prisma commands:
```bash
npx prisma init
npx prisma generate
npx prisma db push
```

#### Stripe

```bash
npm install stripe
```
