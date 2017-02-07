Source for [https://mondotunes.org](https://mondotunes.org)

Migrated from wordpress so there is the odd broken link etc...

<!-- MarkdownTOC -->

- [Building](#building)
  - [Building for s3 deployment](#building-for-s3-deployment)
- [Releasing](#releasing)
- [Jekyl Admin CMS Editor](#jekyl-admin-cms-editor)
- [Points of note](#points-of-note)

<!-- /MarkdownTOC -->




<a name="building"></a>
## Building

Tested against ruby 2.3.3

```bash
gem install bundler
bundle install
jekyll clean
jekyll build
```

<a name="building-for-s3-deployment"></a>
#### Building for s3 deployment

```bash
pip install s3cmd
s3cmd --configure
```

<a name="releasing"></a>
## Releasing

```bash
./deploy_s3.sh
```

<a name="jekyl-admin-cms-editor"></a>
## Jekyl Admin CMS Editor

```bash
jekyll serve
```

Browse to [http://localhost:4000/admin](http://localhost:4000/admin)

<a name="points-of-note"></a>
## Points of note

- Based off https://github.com/daattali/beautiful-jekyll
  - Converted to Jekyll 3
  - Updated bootstrap
  - Moved external font and bootstrap deps to local repo
- Currently hosted off s3, might move to GH pages now that they support Jekyll 3
- Sits behind Cloudflare
