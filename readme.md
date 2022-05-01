# DOM utils

⚠️ WIP ⚠️

## Library usage

### Browser

Library is exported as `DOMore` global variable. Référence in [gulpfile](./gulpfile.js#L17)

### Node

```js
// JavaScript  
const { createElement } = require("domore")

document.body.appendChild(
  createElement(".section > img[src=./img/].card(5)")
)
```

```ts
// TypeScript  
import { createElement } from "domore"

console.log(
  createElement(".section > img[src='./img/{i}.png'].card*5")
)
```

### Result

```html
<div class=section>
  <img src="./img/0.png" class=card/>
  <img src="./img/1.png" class=card/>
  <img src="./img/2.png" class=card/>
  <img src="./img/3.png" class=card/>
  <img src="./img/4.png" class=card/>
</div>
```
