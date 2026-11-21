# Map frontend

An Angular 13 and Leaflet prototype for selecting a point on a map, drawing obstacles and displaying calculation results. It pairs with the Spring Boot service in [`arpesterev/azs_backend`](https://github.com/arpesterev/azs_backend).

## Features visible in the source

- OpenStreetMap tiles displayed through Leaflet.
- Point selection on the map.
- Circle, rectangle and polygon drawing via `leaflet-draw`.
- Coordinates, drawing data and overlays shared between page components.
- A separate backend for radius calculations.

The main screens are `HomeComponent` and `LeafletMapComponent`.

## Run locally

With Node.js and npm installed:

```sh
npm ci
npm start
```

The Angular development server is configured to run at http://localhost:4200. The corresponding backend code allows requests from that origin.

To produce a frontend build:

```sh
npm run build
```

## Source map

- [`src/app/home/`](src/app/home/): control panel and calculation workflow.
- [`src/app/leaflet-map/`](src/app/leaflet-map/): interactive map.
- [`src/models/`](src/models/): map and request models.
- [`src/app/app-routing.module.ts`](src/app/app-routing.module.ts): routes.

This is a research/demo prototype, not an independently validated safety or engineering application. Neither frontend nor backend commands were run during this documentation-only change.
