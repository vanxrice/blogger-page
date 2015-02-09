# &lt;blogger-page&gt;
A Polymer web component that fetches posts from Blogger, displays blog post previews as a grid of cards. Preview cards expand to a full content view and link to the blogger source post.

The response object is exposed as `response`, which enables you to use the response outside of the element.

**Uses Blogger APIv3, which requires an API key. See Google's documentation on how to obtain a Blogger API key (https://developers.google.com/blogger/docs/3.0/using#APIKey).**

Warning: this project uses core-animated-pages, which causes some weird height issues I haven't been able to resolve ([see post on StackOverflow](http://stackoverflow.com/questions/28237391/polymer-core-animated-pages-setting-inside-elements-height-to-0)). This element is best used at the bottom of a page. If you want to embed inside a page, you must set a static height. See the demo.

See the [component page](http://vanxrice.github.io/blogger-page/components/blogger-page) for more information.

If you are interested in using this project, I encourage you to fork and customize to your liking.

## Live demo
See the [demo page](http://vanxrice.github.io/blogger-page/components/blogger-page/demo.html).

## How To Use
### Installation
Available on [Bower](http://bower.io) as **blogger-page**.

Add to bower.json:
```json
{
  "dependencies": {
    "blogger-page": "~0.2.0"
  }
}
```

### Usage
This component is built using [Polymer](https://www.polymer-project.org/) and uses the [Web Component](http://webcomponents.org/) stack.

```html
<!-- … -->
<script src="../webcomponentsjs/webcomponents.js"></script>

<link rel="import" href="bower_components/blogger-page/blogger-page.html">
<!-- … -->
<blogger-page blogId="3730718121569395510" apiKey="yourapikey"
  contentPreviewMaxChars="200" maxPostCount="3">
</blogger-page>
<!-- using data binding: -->
<blogger-page blogId="{{blogId}}" apiKey="{{apiKey}}"></blogger-page>
```

## Maintained by
- Vander Rice (Full-Stack Web Software Engineer)
- Twitter: [@van_rice](http://twitter.com/van_rice)
- Web: [http://vxrice.com](http://vxrice.com)

## License
Apache License Version 2.0, see LICENSE file

Copyright © 2014 [@van_rice](http://twitter.com/van_rice)
