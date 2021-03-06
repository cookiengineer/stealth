
# Refactor

- [ ] Fix `Server` or `SOCKS` Connection, Reviews don't work anymore.

- [ ] Refactor `Request.mjs` with new HTTP Connection API.
- [ ] Move `fix-request` error page to `fix-connection` (as all protocols now use this error in case of socket problems).
- [ ] Refactor `WS` Connection with better encode() and decode() usage (as in DNS and HTTP implementations)

# Notes

These are important notes that need to be revised at a later point in time, but they are technically no issues,
that's why they are collected in here:

- [ ] Clarify whether Win10 crypt32.dll supports `TLS_Method` or really only `SSLv3`.
- [ ] HTTP connection needs support for `Content-Disposition` header to be able to download generated files (e.g. `download.php?id=1337`).
- [ ] HTTP connection needs support for `Content-Location` header to be able to map redirects correctly (e.g. `redirect.php?id=1337`).
- [ ] `Image Optimizers` to compress images on-disk-cache (`optipng`, `libjpeg-turbo`, `convert` from `bmp` to `jpeg`).
- [ ] `Video Optimizers` to compress videos on-disk-cache (convert to `mp4` or `mkv`).



# TODO

- Replace usage of `../base/index.mjs` in stealth/review and use `stealth/extern/base.mjs` instead.

- `/make.mjs` should include browser/make.mjs `build()` and `pack()` with different target folders
- Each make.mjs uses specific folders (/stealth, /browser, /base etc)


