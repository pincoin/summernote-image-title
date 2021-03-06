# summernote-image-title
A plugin for the [Summernote](https://github.com/summernote/summernote/) WYSIWYG editor.

Adds a button to the image popover to edit title and alt attributes.

### Installation

#### 1. Include JS

This plugin is available on Bower:

```
bower install summernote-image-title --save
```

Include the following code after Summernote:

```html
<script src="summernote-image-title.js"></script>
```

#### 2. Supported languages

Currently available in:
- English
- French
- Korean (thanks to [@lqez](https://github.com/lqez) and [@pincoin](https://github.com/pincoin))
- Portuguese (thanks to [@parg-programador](https://github.com/parg-programador))
- Spanish (thanks to Cristian from [Websfrits.com](http://www.websfrits.com/))
- Català (thanks to Cristian from [Websfrits.com](http://www.websfrits.com/))
- German (thanks to [@osworx](https://github.com/osworx))
- Russian (thanks to [@anton-z](https://github.com/anton-z))
- Dutch (thanks to [MysticEarth](https://github.com/MysticEarth))
- Thai (thanks to [@pincoin](https://github.com/pincoin))

Contributions are welcomed!

#### 3. Summernote options

Finally, customize the Summernote image popover.
You can choose if you want to edit the alt attribute specifically or not with the option `specificAltField`:

```javascript
$(document).ready(function() {
    $('#summernote').summernote({
        imageTitle: {
          specificAltField: true,
        },
        lang: 'fr-FR',
        popover: {
            image: [
                ['imagesize', ['imageSize100', 'imageSize50', 'imageSize25']],
                ['float', ['floatLeft', 'floatRight', 'floatNone']],
                ['remove', ['removeMedia']],
                ['custom', ['imageTitle']],
            ],
        },
    });
});
```

### Example

You can see a working example [here](http://codepen.io/asiffermann/pen/EKvMMm).

