# NgMaterial

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.0.6.

```
ng new ng-material  --style=scss
yarn add @angular/material @angular/animations hammerjs
```

add to `angular-cli.json`:

```
"scripts": [
  "../node_modules/hammerjs/hammer.min.js"
],
```

add to `app.module.ts`:

```
import { MaterialModule } from '@angular/material';
import { BrowserAnimationsModule } from '@angular/platform-browser/animations';
```

and

```
imports: [
    ...
    BrowserAnimationsModule,
    MaterialModule
  ],
```

add to `style.scss`

```
@import '~@angular/material/prebuilt-themes/deeppurple-amber.css';
@import url('https://fonts.googleapis.com/icon?family=Material+Icons');

body {
  margin: 0;
  font-family: Roboto, sans-serif;
}
```

then use any material components, for example in `app.component.html`:

<md-toolbar color="primary">
  Angular Material 2 App
</md-toolbar>

<div style="padding: 7px">
  
  <p>
    <button md-button>Basic Button</button>

    <md-slide-toggle>Slide Toggle</md-slide-toggle>
  </p>

</div> 



## Run the app locally
Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

