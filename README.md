# vercel-toast-fork

## Useage

```bash
yarn add vercel-toast-fork -S
```

```js
import 'vercel-toast-fork/dist/vercel-toast.css'
import { createToast } from 'vercel-toast-fork'
createToast('hi，发现新版本可用。', {
  action: {
    text: '立即刷新',
    callback: () => {
      window.location.reload()
    }
  },
  cancel: {
    text: '取消',
    callback: els => {
      els.destory()
    }
  }
})
```
