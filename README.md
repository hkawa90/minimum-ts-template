# minimum-ts-template

## Description

This template use below development tools.
* Emacs/VSCode
* ESLint
* prettier
* parcel
* config
* typescript
(Optional)
 * nyc, mocha, ts-node, espower-typescript, power-assert

ESLint, prettier, parcel, config and typescript is installed by `npm install`.

## Getting Started 

```
git clone https://github.com/hkawa90/minimum-ts-template.git
cd minimum-html5-template
npm install
```

## Setup

### ESLint Environment

Run `eslint --init`

```
npm run init
```
You select ESLint option. Then, created .eslintrc file.

```
? How would you like to configure ESLint? (Use arrow keys)
? What type of modules does your project use? … 
? Which framework does your project use? … 
? Does your project use TypeScript? ‣ No / Yes
? Where does your code run? …  (Press <space> to select, <a> to toggle all, <i> to invert selection)
? What format do you want your config file to be in? … 
? Would you like to install them now with npm? ‣ No / Yes
```

### Prettier Environment

Add eslint-config-prettier to the "extends" array in your .eslintrc.* file. 

```json
{
  "extends": [
    "prettier"
  ]
}
```

### VSCode 

Push `F1` key on VSCode.

```
ext install eslint
ext install prettier
ext install EditorConfig
```

## Customize editor environment

You shoud modfiy below configuration file under your project rule.

* .editorconfig

current configuration:
```
# editorconfig.org

root = true

[*]
charset = utf-8
indent_size = 2
indent_style = space
insert_final_newline = true
trim_trailing_whitespace = true
```

* .eslintrc*

## Structure

```
.
├── css
│   ├── main.css
│   └── normalize.css
├── img
├── js
│   └── main.js
├── node_modules
├── LICENSE
├── README.md
├── index.html
├── package-lock.json
└── package.json
```

* main.css : empty file.
* normalize.css : github.com/necolas/normalize.css v8.0.1
* main.js : empty file.
* index.html : HTML5 html template file.

### index.html

```html
<!DOCTYPE html>
<html class="no-js" lang="*">
<head>
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta charset="utf-8">
<title></title>
<meta name="description" content="*">
<meta name="author" content="*">
<!-- Open Graph Protcol -->
<meta property="og:title" content="*">
<meta property="og:type" content="*">
<meta property="og:url" content="*">
<meta property="og:image" content="*">
<!-- Open Graph Protcol -->
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="shortcut icon" href="*"> <!-- favicon.ico -->
<link rel="apple-touch-icon" href="*"> <!-- touch icons -->
<link rel="stylesheet" href="css/normalize.css">
<link rel="stylesheet" href="css/main.css">

<!--[if lt IE 9]>
<script src="//cdnjs.cloudflare.com/ajax/libs/html5shiv/3.7.2/html5shiv.min.js"></script>
<script src="//cdnjs.cloudflare.com/ajax/libs/respond.js/1.4.2/respond.min.js"></script>
<![endif]-->
</head>
<body>

<!-- Place your content here -->


<!-- SCRIPTS -->
<script src="js/main.js"></script>
<!-- Example: <script src=""></script> -->
</body>
</html>
```

Change above * mark.
