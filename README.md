# Mistral

A minimal blogging theme for Hugo using Tailwind CSS.

## ⚠️ WIP ⚠️

I am creating this theme as an exercise to learn modern concepts in HTML and CSS. This theme is very much a POC.

## Installation

Install Tailwind CSS, PostCSS, etc.

```sh
npm init --yes
npm install --save-dev autoprefixer postcss tailwindcss
```

> - postcss - a tool for transforming CSS with JavaScript
> - postcss-cli - CLI tool to execute Postcss commands in the terminal
> - postcss-import - to resolve the path of an @import rule (not currently used)
> - autoprefixer - helps to add vendor prefixes to CSS
> - tailwindcss - CSS library containing utility class

Add the theme to the `themes` directory:

```sh
git submodule add https://github.com/josephsv96/hugo-theme-mistral themes/mistral
```

To upgrade the theme:

```sh
git submodule foreach git pull
```

Set the theme option to `Mistral` in the `config.toml` file of your Hugo site.

```toml
theme = "Mistral"
```

Start hugo server in production mode

```sh
NODE_ENV=production hugo server -D
```

## References

1. [Hugo, Tailwind & Netlify = <3](https://jamespleger.com/blog/2020/hugo-tailwind-netlify/)
2. [How to add TailwindCSS to your Hugo site](https://dev.to/divrhino/how-to-add-tailwindcss-to-your-hugo-site-529)
