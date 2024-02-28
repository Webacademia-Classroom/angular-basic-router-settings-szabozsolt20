# Practices

## Setup the project

- Set the current directory as the workspace: `code ./ -r`
- Install dependencies: `npm i`
- Run the development server: `npm start`
- Open the product page in the browser: http://localhost:4200
- We will only work on the product page.

## Tasks

- Generate components:
  - HomeComponent: page/home, url: ""
  - InstrumentComponent: page/instrument, url: "instruments"
  - MusicianComponent: page/musician, url: "musicians"
  - MusicianEditComponent: page/musician-edit, url: "musicians/edit/:id"
  - AboutComponent: page/about, url: "about"
  - NotFoundComponent: page/not-found, url: "**"
- Setup router in the [app.routes.ts](src/app/app.routes.ts):
  - HomeComponent with preloading
  - InstrumentComponent with preloading
  - MusicianComponent with preloading
  - AboutComponent with preloading
  - NotFoundComponent with preloading

## Testing

- `npm test`

## Further helps

### Setting up routes

- Generating an Angular component:

```cmd
ng g c page/about
```

- Setting up a preloaded route in the app.routes.ts file:

```typescript
{
  path: "about",
  component: AboutComponent,
},
```
