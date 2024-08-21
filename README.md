# Nuxt 3 + ArkUI import issue reproduction

## Steps to reproduce
1. run `pnpm i`
2. run `pnpm dev` and visit `http://localhost:3000/`
3. you now shoul see the error **`500`** `The requested module '../../node_modules/@zag-js/utils/dist/index.js' does not provide an export named 'omit'`
4. if you go to `app.vue` and remove the line `import { Dialog } from "@ark-ui/vue";` the error will be gone
