<!-- tyhp-readme:start -->
# tyhpdef/laravel-passport

Tyhp type definitions for `laravel/passport` `13.8.0`.

```bash
composer require --dev tyhpdef/laravel-passport:13.8.0
```

This is a metapackage. Composer also installs `tyhpdef/laravel-passport-impl` (type files).
Require **this** name, not `tyhpdef/laravel-passport-impl`.

See https://tyhplang.com.

## Maintain `laravel/passport`? Ship the types yourself

If you are a Packagist maintainer of `laravel/passport`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/laravel-passport-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `laravel/passport` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/laravel-passport": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `laravel/passport` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `laravel/passport` with a real constraint,
   `"replace": { "tyhpdef/laravel-passport": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `laravel/passport` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/laravel-passport` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
