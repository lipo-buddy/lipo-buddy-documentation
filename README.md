![Lipo Buddy Documentation Website](/site-image.png)

This is the source code that runs the [Lipo Buddy documentation website](https://docs.lipobuddy.com/).

## How to Contribute

- If you have a request for expanded documentation or question that is not answered in the docs, please open an issue!
- For bug reports or feature requests for the LiPo Buddy ecosystem, please refer to the [lipo-buddy/lipo-buddy-support](https://github.com/lipo-buddy/lipo-buddy-support) repository.
- PRs or issues are welcome for any expanded documentation, spelling/grammar issues, or factual errors.

---

## Developer's Guide

This repository uses Hugo to generate a static site from markdown files. The project also includes a custom theme, specifically designed for the documentation site. The theme sets up sidebar menus, headers and footers, etc.

The site is deployed using Netlify; The `master` branch is deployed to the production site and the `develop`
branch is deployed to the development site.

### Deploy Status

|Branch|Deploy Status|Target|
|------|-------------|------|
|`master`|![Netlify Status](https://api.netlify.com/api/v1/badges/cf816beb-2989-43b9-8499-720df8d1ee2f/deploy-status)|https://docs.lipobuddy.com/|

### Development

Please install [Hugo](https://gohugo.io/).

To run a development server, use: 
```
hugo serve
```

To build and export the site to static HTML, use:
```
hugo
````

This will build the static site to the `public/` directory as HTML. These files should not be uploaded to git; they are ignored and will be built by Netlify during the automated deployment.