See https://github.com/dependabot/dependabot-core/issues/9684

---

`dependabot-log-with-package-manager.txt` contains the log after recreating a PR (`@dependabot recreate`) with `"packageManager": "pnpm@9.3.0"` in `package.json`.\
This correctly updates the package without downgrading the lockfile.

`dependabot-log-without-package-manager.txt` contains the log after recreating a PR (`@dependabot recreate`) without `"packageManager"` in `package.json`.\
This incorrectly downgraded the lcokfile to v6.
