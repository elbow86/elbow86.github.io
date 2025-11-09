# elbow86.github.io

I followed the guide from Burke Holland ([Burke Holland's blogpost](https://burkeholland.github.io/posts/gh-pages-best-blog/)) to get the improved Github Pages site building and deploying. After some troubleshooting it's working now.

What I changed
- Tidied the site structure and confirmed the basic Jekyll build works locally and on GitHub Pages.

Notes & next steps
- Post cadence: decide on a regular publishing rhythm that fits your schedule (weekly, biweekly, monthly). Draft posts locally, then commit and push when ready.
- Gemfile / remote builds: GitHub Pages builds use a limited set of plugins. If you see build errors after pushing, either (a) use the `github-pages` gem so the remote environment matches your local setup, or (b) build the site locally and push the generated `_site` to the `gh-pages` branch or configure a GitHub Action to run `bundle exec jekyll build` and deploy.
- Local tips:
	```bash
	cd elbow86.github.io
	bundle install
	bundle exec jekyll serve
	```
	Preview locally: [Open local preview](http://127.0.0.1:4000).

	Or, if your environment exposes a different port (for example `4001`), open that URL instead.
