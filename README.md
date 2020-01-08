# vue-eulerian

## Install

```bash
# with npm
npm i vue-eulerian
# with yarn
yarn add vue-eulerian
```

In file `main.js`

```js
import Vue from 'vue'
import VueEulerian from 'vue-eulerian'

// VueEulerian
Vue.use(VueEulerian, { id: 'ac.acadomia.fr' })
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
