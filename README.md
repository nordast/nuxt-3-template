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
## Self documentation:
###

#### Install Latest Nuxt Project:

```bash
npx nuxi@latest init <project-name>
```

#### Install Nuxt Color Mode:

```bash
npx nuxi module add color-mode
```

#### Shadcn Setup:

[Documentation](https://www.shadcn-vue.com/docs/installation/nuxt.html)

```bash
npm install -D typescript

npx nuxi@latest module add @nuxtjs/tailwindcss

npx nuxi@latest module add shadcn-nuxt
```

Update the nuxt.config.ts as following:

 ```bash
export default defineNuxtConfig({
  modules: ['@nuxtjs/tailwindcss', 'shadcn-nuxt'],
  shadcn: {
    prefix: '',
    componentDir: './components/ui'
  }
})
```

Run the CLI:

 ```bash
npx shadcn-vue@latest init
 ```

Let's run the following command to install first component:

```bash
npx shadcn-vue@latest add button
 ```

#### VueUse

[Documentation](https://vueuse.org/guide/#nuxt)

```bash
npx nuxi@latest module add vueuse
```