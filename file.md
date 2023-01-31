---
layout: docs
title: Get started with Bootstrap
description: Bootstrap is a powerful, feature-packed frontend toolkit. Build anything—from prototype to production—in minutes.
group: getting-started
aliases:
  - "/docs/5.3/getting-started/"
  - "/docs/getting-started/"
  - "/getting-started/"
toc: true
---

## Quick start

Get started by including Bootstrap's production-ready CSS and JavaScript via CDN without the need for any build steps. See it in practice with this [Bootstrap CodePen demo](https://codepen.io/team/bootstrap/pen/qBamdLj).

<br>

1. **Create a new `index.html` file in your project root.** Include the `<meta name="viewport">` tag as well for [proper responsive behavior](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag) in mobile devices.

   ```html
   <!doctype html>
   <html lang="en">
     <head>
       <meta charset="utf-8">
       <meta name="viewport" content="width=device-width, initial-scale=1">
       <title>Bootstrap demo</title>
     </head>
     <body>
       <h1>Hello, world!</h1>
     </body>
   </html>
   ```

2. **Include Bootstrap's CSS and JS.** Place the `<link>` tag in the `<head>` for our CSS, and the `<script>` tag for our JavaScript bundle (including Popper for positioning dropdowns, poppers, and tooltips) before the closing `</body>`. Learn more about our [CDN links](#cdn-links).

   ```html
   <!doctype html>
   <html lang="en">
     <head>
       <meta charset="utf-8">
       <meta name="viewport" content="width=device-width, initial-scale=1">
       <title>Bootstrap demo</title>
       <link href="{{< param "cdn.css" >}}" rel="stylesheet" integrity="{{< param "cdn.css_hash" >}}" crossorigin="anonymous">
     </head>
     <body>
       <h1>Hello, world!</h1>
       <script src="{{< param "cdn.js_bundle" >}}" integrity="{{< param "cdn.js_bundle_hash" >}}" crossorigin="anonymous"></script>
     </body>
   </html>
   ```

   You can also include [Popper](https://popper.js.org/) and our JS separately. If you don't plan to use dropdowns, popovers, or tooltips, save some kilobytes by not including Popper.

   ```html
   <script src="{{< param "cdn.popper" >}}" integrity="{{< param "cdn.popper_hash" >}}" crossorigin="anonymous"></script>
   <script src="{{< param "cdn.js" >}}" integrity="{{< param "cdn.js_hash" >}}" crossorigin="anonymous"></script>
   ```

3. **Hello, world!** Open the page in your browser of choice to see your Bootstrapped page. Now you can start building with Bootstrap by creating your own [layout]({{< docsref "/layout/grid" >}}), adding dozens of [components]({{< docsref "/components/buttons" >}}), and utilizing [our official examples]({{< docsref "/examples" >}}).

## CDN links

As reference, here are our primary CDN links.

{{< bs-table >}}
| Description | URL |
| --- | --- |
| CSS | `{{< param "cdn.css" >}}` |
| JS | `{{< param "cdn.js_bundle" >}}` |
{{< /bs-table >}}

You can also use the CDN to fetch any of our [additional builds listed in the Contents page]({{< docsref "/getting-started/contents" >}}).

## Next steps
