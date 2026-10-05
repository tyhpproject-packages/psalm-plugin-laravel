<!-- tyhp-readme:start -->
# tyhpdef/psalm-plugin-laravel

Tyhp type definitions for `psalm/plugin-laravel` `4.16.1`.

```bash
composer require --dev tyhpdef/psalm-plugin-laravel:4.16.1
```

This is a metapackage. Composer also installs `tyhpdef/psalm-plugin-laravel-impl` (type files).
Require **this** name, not `tyhpdef/psalm-plugin-laravel-impl`.

See https://tyhplang.com.

## Maintain `psalm/plugin-laravel`? Ship the types yourself

If you are a Packagist maintainer of `psalm/plugin-laravel`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/psalm-plugin-laravel-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `psalm/plugin-laravel` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/psalm-plugin-laravel": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `psalm/plugin-laravel` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `psalm/plugin-laravel` with a real constraint,
   `"replace": { "tyhpdef/psalm-plugin-laravel": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `psalm/plugin-laravel` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/psalm-plugin-laravel` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
