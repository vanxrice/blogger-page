&lt;blogger-page&gt;
============

See the [component page](http://vanxrice.github.io/blogger-page/components/blogger-page) for more information.

## Live demo
See the [demo page](http://vanxrice.github.io/blogger-page/components/blogger-page/demo.html).

> A basic Polymer web component that fetches posts from Blogger over JSON. Displays blog post preview as a cards, which expand to a full content preview and link to the blogger source post. Uses Blogger APIv3, which requires an API key. See Google's documentation on how to obtain a Blogger API key (https://developers.google.com/blogger/docs/3.0/using#APIKey).

> Warning: this project uses core-animated-pages, which causes some weird height issues I haven't been able to resolve ([see post on StackOverflow](http://stackoverflow.com/questions/28237391/polymer-core-animated-pages-setting-inside-elements-height-to-0)). This element is best used at the bottom of a page. If you want to embed inside a page, you must set a static height. See the demo.

## How To Use
Add to bower.json:
```json
{
  "dependencies": {
    "blogger-page": "~0.1.0"
  }
}
```
```html
<link rel="import" href="../blogger-page/blogger-page.html">
<!-- ... -->
<blogger-page blogtitle="vxrice"></blogger-page>
```

## Maintained by
- Vander Rice (Full-Stack Web Software Engineer)
- Twitter: [@van_rice](http://twitter.com/van_rice)
- Web: [http://vxrice.com](http://vxrice.com)

## License
Apache License Version 2.0, see LICENSE file

Copyright (c) 2014 [@van_rice](http://twitter.com/van_rice)
