Now L-Admin is supported with ViteJs and no longer uses Laravel Mix. You only need to install the Node.js module in your module directory and then run ViteJs as usual.

Change directory to the module path:

```bash
cd Modules/Blog
```

The default `package.json` file includes everything you need to get started. You may install the dependencies it references by running:
```bash
$ npm install
```

# Running ViteJs

To run ViteJs you only need to execute one of the NPM scripts that is included with the default **Ladmin** `package.json` file

```bash
// Run ViteJs
$ npm run dev

// Run all ViteJs and minify output...
$ npm run build
```

After the asset version is created, you need to call it in the layout file that you have provided previously by:
```html
<head>
    . . . 

    @vite([
        'Modules/Blog/Resources/js/blog.js',
        'Modules/Blog/Resources/css/blog.css'
    ])
    
    . . . 
</head>

```

For more info on Asset Bundling (Vite) view the documentation here: [https://laravel.com/docs/master/vite](https://laravel.com/docs/10.x/vite)