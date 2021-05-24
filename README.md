# Digital garden Jekyll template
Demo: [megumi.website](https://megumi.website)

Powered by: Github --> DeployHQ --> Dreamhost

### General Template Updates
- Updated `site.baseurl` in `head.html` metadata, added `.html` conditional clause, removed `site.url` variable
- Forked Last Modified plugin to my own account & deleted stale branches
- Added timezone to `_config.yml` for Last Modified plugin to work
- Removed relative permalinks due to error I got in [my GH Pages repo](https://github.com/meewgumi/digital-garden-ghpages/commits/main)
- Renamed `notes-graph` for the same reason as above
- Added variable in `_config.yml` for `show_notes_graph` and set to `false` by default
- Created `archive.md` with automatic list of all notes
- Added back `site.url` and configured metadata accordingly. `baseurl` is now the subdirectory, blank by default
- 

### Apache Specific Updates
- Need to force `.html` extension for this to work on Dreamhost
  - I chose not to pursue the `.htaccess` option to remove extensions, since it requires `link rel=canonical` on every page. As a result, I removed all canonical metadata from note headers.
- Renamed all links and pages to follow `.html` scheme
- Added `.htaccess` for 404
- Moved all files from `_pages` to root directory because they weren't being built in my deployment actions
	- As a result, no longer need Permalink front matter or the config section for `_pages`
- Configured [Jekyll Build Commands](https://www.deployhq.com/guides/jekyll) and `vendor` caching on [DeployHQ](https://www.deployhq.com/r/nx7qct)
- Added comment in `_config.yml` making it easy to hide `.htaccess` include to make this compatible with non-Apache servers

### Notes
With these changes, this template would work on any Apache host via [DeployHQ](https://www.deployhq.com/r/nx7qct). I chose DeployHQ because it's owned by Krystal UK and runs on 100% renewable energy.

Must use an apex domain or subdomain. I got errors with the base URL when attempting to use a subdirectory.

## License
[Original Jekyll template](https://github.com/maximevaillancourt/digital-garden-jekyll-template) is available under the [MIT license](LICENSE.md).
