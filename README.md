# CloudReader.app documentation

A documentation site powered by Eleventy & Tailwind CSS.
You can see a demo at https://cloudreader.app/

## Getting started

1. Clone this repository

```shell
git clone https://github.com/cloudreaderapp/cloudreaderdoc.git documentation
```

2. Go into this new folder

```shell
cd documentation
```

3. Install dependencies

```shell
npm install
```

4. Tailwind initial build

```shell
npx tailwindcss -i src/assets/css/index.css -c tailwind.config.js -o _site/index.css --minify
```

### Development

```shell
npm run dev
```


### Production

```shell
npm run build
```


### Configuring

To change title, description, etc. Update file ``metadata.json`` in ``_data`` directory.
Add your documents (pages) in ``_docs``

## Credits
- [Eleventy Static Site Generator](https://www.11ty.dev/)
- [Tailwind](https://tailwindcss.com/)
- [Documentation theme built with Tailwind CSS](https://spinalcms.com/resources/11ty-documentation-theme-with-tailwind-css/)

## Contributing

1. Fork it (https://github.com/cloudreaderapp/cloudreaderdoc.git)
2. Clone the fork using `git clone` to your local development machine.
3. Create your feature branch (`git checkout -b my-new-feature`)
4. Commit your changes (`git commit -am 'Add some feature'`)
5. Push to the branch (`git push origin my-new-feature`)
6. Create a new Pull Request
