# quilljs-image-buttons
Overlay image buttons for quill

![](https://s.hinty.io/W3owGBk5XoGtCvJc3x9kYi.png)

```js
import Quill from 'quill';
import { imageButtons } from 'quilljs-image-buttons';

Quill.register('modules/imageButtons', imageButtons);

const quill = new Quill(editor, {
    modules: {
        imageButtons: [
          html: '<button>Edit</button>',
          callback: function(imageSrc, replaceImage) {
             replaceImage(new_image_src)
          },
        ],
    }
});
```
