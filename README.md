<!-- tyhp-readme:start -->
# tyhpdef/twig-twig

Tyhp type definitions for `twig/twig` `3.28.0`.

```bash
composer require --dev tyhpdef/twig-twig:3.28.0
```

This is a metapackage. Composer also installs `tyhpdef/twig-twig-impl` (type files).
Require **this** name, not `tyhpdef/twig-twig-impl`.

See https://tyhplang.com.

## Maintain `twig/twig`? Ship the types yourself

If you are a Packagist maintainer of `twig/twig`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/twig-twig-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `twig/twig` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/twig-twig": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `twig/twig` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `twig/twig` with a real constraint,
   `"replace": { "tyhpdef/twig-twig": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `twig/twig` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/twig-twig` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
