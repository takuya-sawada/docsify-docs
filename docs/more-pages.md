# More pages

If you need more pages, you can simply create more markdown files in your docsify directory. If you create a file named `guide.md`, then it is accessible via `/#/guide`.

For example, the directory structure is as follows:

```text
.
└── docs
    ├── README.md
    ├── guide.md
    └── zh-cn
        ├── README.md
        └── guide.md
```

Matching routes

```text
docs/README.md        => http://domain.com
docs/guide.md         => http://domain.com/#/guide
docs/zh-cn/README.md  => http://domain.com/#/zh-cn/
docs/zh-cn/guide.md   => http://domain.com/#/zh-cn/guide
```

## Sidebar

In order to have a sidebar, you can create your own `_sidebar.md` (see [this documentation's sidebar](https://github.com/docsifyjs/docsify/blob/master/docs/_sidebar.md) for an example):

First, you need to set `loadSidebar` to **true**. Details are available in the [configuration paragraph](configuration.md#loadsidebar).

```html
<!-- index.html -->

<script>
  window.$docsify = {
    loadSidebar: true,
  };
</script>
<script src="//cdn.jsdelivr.net/npm/docsify/lib/docsify.min.js"></script>
```

Create the `_sidebar.md`:

```markdown
<!-- docs/_sidebar.md -->

- [Home](/)
- [Guide](guide.md)
```

You need to create a `.nojekyll` in `./docs` to prevent GitHub Pages from ignoring files that begin with an underscore.

!> Docsify only looks for `_sidebar.md` in the current folder, and uses that, otherwise it falls back to the one configured using `window.$docsify.loadSidebar` config.

Example file structure:

```text
└── docs/
    ├── _sidebar.md
    ├── index.md
    ├── getting-started.md
    └── running-services.md
```
