If you want to change the style, or add a script to the **Ladmin** module, you can start by going to the **Ladmin** directory.

```bash
cd Modules/Ladmin && npm install
```

Run ViteJs in root project directory
```bash
npm run dev
```

## Change Accent Color

You can also change the accent color of the **Ladmin** template, open the file `Modules/Ladmin/Resources/scss/_variable.scss` and after that change the variable `$primary` with the color you want.
```scss
. . .

$primary:       #6f42c1; // purple

. . .
```

![Green Dashboard](https://raw.githubusercontent.com/hexters/assets/main/ladmin/v3/captures/home-purple.png)

You can also add some feature by add other package, for example adding `vue`, `Laravel Echo`, etc.