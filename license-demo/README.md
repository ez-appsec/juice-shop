# License inventory demo

This isolated scan fixture records `vm2@3.9.17` and its transitive dependencies
in an npm-generated lockfile. It supplies exact package versions, integrity
hashes and public npm registry URLs for a fresh SourceBastion inventory and
license-catalog demonstration in the current project view.

It reuses the intentionally vulnerable package from SourceBastion's scanner
fixture corpus. It is scan input only; it is not imported by Juice Shop or
installed by the application build. No dependency installation is needed to
scan these files.

The lockfile was generated with npm 11.8.0 using:

```sh
npm install --package-lock-only --lockfile-version=3 --ignore-scripts --no-audit --no-fund
```

After this change is merged and the current revision is scanned, open the
project's SBOM and filter project root to `license-demo`. Scan-input license
claims and public-catalog observations remain separate. Catalog observations
require the development demand export, catalog refresh and snapshot freeze.

The scanner currently reports npm engine constraints as unsupported selection
controls. The exact locked rows and provenance are retained, but this fixture
does not establish complete runtime activation or selection coverage.
