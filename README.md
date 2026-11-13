# Garak's Shop VPM

VPM (VRChat Package Manager) listing for the VRChat Creator Companion (VCC). Packages by Garak's Shop are listed here; the listing itself is built by GitHub Actions from [`source.json`](source.json) and published on GitHub Pages.

## Add to VCC

- Listing URL: `https://hyde4280.github.io/garakshop-vpm/index.json`
- One click: [Add to VCC](vcc://vpm/addRepo?url=https%3A%2F%2Fhyde4280.github.io%2Fgarakshop-vpm%2Findex.json)
- Or in the VCC: Settings > Packages > Add Repository, then paste the listing URL.

## Packages

None are listed yet. Planned: `jp.garakshop.cellloader`, `jp.garakshop.elevator`, `jp.garakshop.shower`. Each package lives in its own public repository (released from a development repository with `git subtree split`) and is added to `githubRepos` in `source.json`.

## Updating the listing

The listing is **not** rebuilt automatically when a package publishes a new release. After a release, run the "Build Repo Listing" workflow by hand (Actions > Build Repo Listing > Run workflow), or push a change to `source.json` on `main`.

To add a package, put its GitHub repository (`owner/name`, with a Release that has the package zip) into `githubRepos` in `source.json` and push to `main`.

## License

The listing files are provided under the MIT License; each package has its own license (MIT unless stated otherwise in its repository).
