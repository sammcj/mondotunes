## source for mondotunes.org website

mondotunes.org used to be a wordpress site, I've converted all the posts to markdown, added the required jekyll markup, cleaned a few of the youtube embedding code up, then re-released as a jekyll generated static page.

Expect bugs etc...

## Releasing

Requires s3 API keys etc...

```
./deploy_s3.sh
```

## Points of note

- Based off https://github.com/daattali/beautiful-jekyll
  - Converted to Jekyll 3
  - Updated bootstrap
  - Moved external font and bootstrap deps to local repo
- Currently hosted off s3, might move to GH pages now that they support Jekyll 3
- Sits behind Cloudflare
