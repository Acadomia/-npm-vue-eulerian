# -npm-vue-eulerian

forked from [tomderudder/vue-eulerian](https://gitlab.com/tomderudder/vue-eulerian)

## Install

```bash
# with npm
npm i @acadomia/vue-eulerian
# with yarn
yarn add @acadomia/vue-eulerian
```

In file `main.js`

```js
import Vue from 'vue'
import VueEulerian from 'vue-eulerian'

// VueEulerian
Vue.use(VueEulerian, { id: process.env.EULERIAN_ACCOUNT_ID })
```

## Usage

In `.vue` file

```js
export default {
  name: 'myPageComponent',

  created() {
    // for add tag on page load event
    this.$eulerian.push(
      'parametre1',
      'valeur1',
      'parametre2',
      'valeur2',
      'parametre3',
      'valeur3'
    )
  },

  methods: {
    submitForm() {
      // for add tag on page custom event
      this.$eulerian.push(
        'parametre1',
        'valeur1',
        'parametre2',
        'valeur2',
        'parametre3',
        'valeur3'
      )
    }
  }
}
```
