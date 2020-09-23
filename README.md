# stable-starter

> Get a jump start building Drupal 8 and 9 themes using Stable Starter, a sub-theme of [Stable](https://www.drupal.org/docs/8/core/themes/stable-theme).

## Installation

### Install via Composer (recommended)

In Drupal project root, run `omposer create-project bmarshall511/stable_starter themes/custom/stable-starter dev-master`

### Install Manually

1. Download the theme.
2. Upload the *stable-starter* folder to the desired themes folder in your Drupal installation.
3. Download [gulp-starter](https://github.com/bmarshall511/gulp-starter).
4. Upload the *gulp-starter* folder the the *stable-starter* theme folder and rename it to `assets`.
5. Install the required node modules in the assets folder by running `npm install` inside the directory.
6. Enable and make it the active, default theme.

## Development

For information on developing and compiling resources within the *assets* folder, see the [gulp-starter README.md](https://github.com/bmarshall511/gulp-starter/blob/master/README.md).

### Theme Libraries

* `stable_starter/stable_starter` - Includes the global, base [non-critical](https://web.dev/defer-non-critical-css/) CSS styles.

### Required Modules

* [Critical CSS](https://www.drupal.org/project/critical_css) - Embeds a critical CSS file into a page's HTML head, and loads the rest of non-critical CSS asynchronously.

## Deployment Checklist

- [ ] Update the *favicon.ico*.
- [ ] Update the *logo.svg*.
- [ ] Update the *screenshot.png*.
- [ ] Compile *assets* for production by running `npm run build`.
- [ ] If using a git repo, remove `assets` from the *.gitignore* file.
