# Weatherverse Frontend

The published build of the Weatherverse weather application's front end. It is a Blazor WebAssembly app (page title `wasm`), compiled and ready to be served as static files. This repo has no C# or Razor source code.

## What is in this repo

- `_framework/`: the compiled Blazor WebAssembly runtime and app assemblies (including `Blazored.LocalStorage` and the ASP.NET Core authorization libraries).
- `index.html`, `service-worker.js`, `manifest.webmanifest`: the app shell and its progressive web app files.
- `data/cities.json`, `sample-data/weather.json`, `appsettings.json`: data and configuration files.
- `images/` and `css/`: images and styles used by the app.
- `404.html` and `.nojekyll`: files used when hosting on GitHub Pages.
- `.github/workflows/dotnet.yaml`: a GitHub Actions workflow.

The `index.html` sets its base path to `/weatherverse-wasm/`.

## Hosting

GitHub Pages is enabled for this repo: https://jvishwa06.github.io/weatherverse-frontend/

The app talks to the Weatherverse backend API. The backend is in [weatherverse-backend](https://github.com/jvishwa06/weatherverse-backend), and a newer version is in [identity-auth-api](https://github.com/jvishwa06/identity-auth-api).
