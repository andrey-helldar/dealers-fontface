# dealers-fontface

Set of official dealer fonts in SCSS.

![dealers-fontface](https://user-images.githubusercontent.com/10347617/43892308-45fc1eb8-9bd4-11e8-8659-6ae4301658cd.png)

<p align="center">
    <a href="https://yarn.pm/dealers-fontface"><img src="https://img.shields.io/npm/dt/dealers-fontface.svg?style=flat-square" alt="Total Downloads" /></a>
    <a href="https://yarn.pm/dealers-fontface"><img src="https://img.shields.io/npm/v/dealers-fontface.svg?style=flat-square" alt="Latest Stable Version" /></a>
    <a href="LICENSE"><img src="https://img.shields.io/npm/l/dealers-fontface.svg?style=flat-square" alt="License" /></a>
</p>

## Installation

**NPM**
```bash
npm i --save-dev dealers-fontface
```

**Yarn**
```
yarn add --dev dealers-fontface
```


## What does it do?

The package contains official fonts of dealers:

 * [Cars](#cars)
    * [Ford](#ford)
    * [Hyundai](#hyundai)
    * [Isuzu](#isuzu)
    * [Mercedes-Benz](#mercedes-benz)
    * [Mitsubishi](#mitsubishi)

### Cars

#### Ford
```css
.ford-antenna-black     { font-family: 'FordAntenna'; font-weight: 900; font-style: normal; }
.ford-antenna-bold      { font-family: 'FordAntenna'; font-weight: 700; font-style: normal; }
.ford-antenna-semibold  { font-family: 'FordAntenna'; font-weight: 600; font-style: normal; }
.ford-antenna-medium    { font-family: 'FordAntenna'; font-weight: 500; font-style: normal; }
.ford-antenna-regular   { font-family: 'FordAntenna'; font-weight: 400; font-style: normal; }
.ford-antenna-light     { font-family: 'FordAntenna'; font-weight: 300; font-style: normal; }

.ford-antenna-comp-black { font-family: 'FordAntennaComp'; font-weight: 900; font-style: normal; font-stretch: extra-condensed; }

.ford-antenna-cond-bold     { font-family: 'FordAntennaCond'; font-weight: 700; font-style: normal; }
.ford-antenna-cond-medium   { font-family: 'FordAntennaCond'; font-weight: 500; font-style: normal; }
.ford-antenna-cond-regular  { font-family: 'FordAntennaCond'; font-weight: 400; font-style: normal; }
```

#### Hyundai
```css
.hyundai-sans-head-bold    { font-family: 'HyundaiSansHead'; font-weight: 700;    font-style: normal; font-size: 30px; }
.hyundai-sans-head-medium  { font-family: 'HyundaiSansHead'; font-weight: 500;    font-style: normal; font-size: 30px; }
.hyundai-sans-head-regular { font-family: 'HyundaiSansHead'; font-weight: normal; font-style: normal; font-size: 30px; }
.hyundai-sans-head-light   { font-family: 'HyundaiSansHead'; font-weight: 300;    font-style: normal; font-size: 30px; }

.hyundai-sans-text-bold          { font-family: 'HyundaiSans'; font-weight: 600;    font-style: normal; }
.hyundai-sans-text-bold-italic   { font-family: 'HyundaiSans'; font-weight: 600;    font-style: italic; }
.hyundai-sans-text-medium        { font-family: 'HyundaiSans'; font-weight: 500;    font-style: normal; }
.hyundai-sans-text-medium-italic { font-family: 'HyundaiSans'; font-weight: 500;    font-style: italic; }
.hyundai-sans-text-italic        { font-family: 'HyundaiSans'; font-weight: normal; font-style: italic; }
.hyundai-sans-text-regular       { font-family: 'HyundaiSans'; font-weight: normal; font-style: normal; }
```

#### Isuzu
```css
.isuzu-expand { font-family: 'Usuzi Expanded'; font-weight: normal; font-style: normal; }
``` 

#### Mercedes-Benz
```css
.mercedes-benz-cac-regular { font-family: 'Corporate A Condensed'; font-weight: 400; font-size: 30px; }
.mercedes-benz-cs-regular  { font-family: 'Corporate S Regular';   font-weight: 400; }
.mercedes-benz-cs-demi     { font-family: 'Corporate S Bold';      font-weight: 600; }
```

#### Mitsubishi
```css
.mitsubishi-regular { font-family: 'Bitsumishi'; font-weight: 400; font-style: normal; }
```

And see [test.html](dist/test.html) as example.

## Using

### SCSS
You can use certain fonts pack in your application:
```scss
@import "~dealers-fontface/src/scss/dealers/ford";
@import "~dealers-fontface/src/scss/dealers/hyundai";
@import "~dealers-fontface/src/scss/dealers/isuzu";
@import "~dealers-fontface/src/scss/dealers/mercedes-benz";
@import "~dealers-fontface/src/scss/dealers/mitsubishi";
```

Or connect a specific font. For example:
```scss
@import "~dealers-fontface/src/scss/dealers/mercedes-benz/corporate-a-condensed";
@import "~dealers-fontface/src/scss/dealers/hyundai/hyundai-sans-head-regular";
@import "~dealers-fontface/src/scss/dealers/ford/fordantennacond-regular";
```

### CSS
Copy the folders `dist/css` and `dist/fonts` to root dir of your project and connect them:
```html
<head>
    <!-- ... -->
    
    <link href="/css/dealers-fontface.css" rel="stylesheet" media="screen,projection">
</head>
```

Also, you can use certain fonts pack in your application:
```html
<head>
    <!-- ... -->
    
    <link href="/css/ford.css" rel="stylesheet" media="screen,projection">
    <link href="/css/hyundai.css" rel="stylesheet" media="screen,projection">
    <link href="/css/isuzu.css" rel="stylesheet" media="screen,projection">
    <link href="/css/mercedes-benz.css" rel="stylesheet" media="screen,projection">
    <link href="/css/mitsubishi.css" rel="stylesheet" media="screen,projection">
</head>
```


# Contributors

You can easily add any official dealer fonts by following the steps.

For example, add fonts `Mercedes-Benz`:

1. Create `mercedes-benz` folder in `src/fonts` and storing files:
```
src/fonts/mercedes-benz/DaimlerCAC/
    DaimlerCAC-Regular.eot
    DaimlerCAC-Regular.svg
    DaimlerCAC-Regular.ttf
    DaimlerCAC-Regular.woff
    DaimlerCAC-Regular.woff2

src/fonts/mercedes-benz/DaimlerCS-Regular/
    DaimlerCS-Regular.eot
    DaimlerCS-Regular.svg
    DaimlerCS-Regular.ttf
    DaimlerCS-Regular.woff
    DaimlerCS-Regular.woff2
```


## License

This package is released under the [MIT License](LICENSE).
