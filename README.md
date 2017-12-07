# Google / G Suite Browserslist Shared Config

This configuration reflects Google's supported browser policy for their suite of web applications.

## What is Browserslist?

Share browsers list between different front-end tools, like Autoprefixer, Stylelint and babel-preset-env.

* [Browserslist](https://github.com/ai/browserslist) (Github repo)
* [browserl.ist](http://browserl.ist) (Browserslist query syntax validation)
* ["Browserslist is a Good Idea"](https://css-tricks.com/browserlist-good-idea/) (blog post by [@chriscoyier](https://github.com/chriscoyier))

## Browser support

You can review the current interpretation of this configuration at [browserl.ist](http://browserl.ist/?q=last+2+Chrome+major+versions%2C+last+2+Firefox+major+versions%2C+last+2+Safari+major+versions%2C+last+2+Edge+major+versions%2C+ie+11%2C+last+3+ChromeAndroid+major+versions%2C+last+2+iOS+major+versions).

As of December 2017, these browsers are supported by default configuration:

### Desktop browsers [[policy](https://support.google.com/a/answer/33864)]

* Chrome 62
* Chrome 61
* Edge 16
* Edge 15
* Firefox 56
* Firefox 55
* IE 11 _(can be excluded via `browserslist-config-google/no-ie`)_
* Safari 11
* Safari 10.1
* Safari 10

### Mobile [[policy](https://support.google.com/a/answer/6288871)]

* Chrome for Android 61
* iOS Safari 11
* iOS Safari 10.3
* iOS Safari 10.0-10.2

## Usage

### package.json

```json
{
  "browserslist": [
    "extends browserslist-config-google"
  ]
}
```

## Alternative configuration

Last `n` versions or `>= [version]`

| Config | Chrome | Firefox | Safari | Edge | IE  | ChromeAndroid | iOS |
| :----- | :----: | :-----: | :----: | :--: | :-: | :-----: | :-: |
| `browserslist-config-google` | 1 | 2 | 2 | 2 | 1 | 3 | 2 |
| `browserslist-config-google/no-ie` | 1 | 2 | 2 | 2 | 0 | 3 | 2 |
| `browserslist-config-google/gdocs` | 2 | 2 | 2 | 2 | 2 | _>= 30_ | _>= 9_ |
