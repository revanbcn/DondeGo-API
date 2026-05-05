## First real use case

The first live use case of the DondeGo API powers daily event selections for:

- Barcelona: https://x.com/HoyBcn
- Madrid: https://x.com/EnMadridHoy

If you are building a project around events, culture, maps, newsletters or local discovery in Barcelona or Madrid, we can share the data for free. Please link back to DondeGo as the source.

# DondeGo API

Local events and places for Barcelona and Madrid.

DondeGo is a city guide focused on helping people discover what to do today, what is happening nearby, and which places are worth knowing in [Barcelona](https://dondego.es/barcelona/) and [Madrid](https://dondego.es/madrid/).

This API is built for developers, media projects, local products, maps, newsletters, and partners who want structured access to urban content with real editorial value.

## What you can get

- Events by city, date, category, and location
- Places near a specific point
- Events inside a given radius
- Structured local content for guides, maps, apps, and editorial products

## Example use cases

### Events today in Madrid

Same idea as the public page for [eventos de hoy en Madrid](https://dondego.es/madrid/eventos/?date=hoy).

```http
GET /api/v1/events/?location=madrid&date=hoy
```

### Events near a point on the map

```http
GET /api/v1/events/?lat=40.4168&lon=-3.7038&radius=3000&date=hoy
```

Example: events today within 3 km of central Madrid.

### Places inside a given radius

```http
GET /api/v1/places/?lat=41.3874&lon=2.1686&radius=2000
```

Example: places within 2 km of central Barcelona.

### Filter by city and category

```http
GET /api/v1/events/?location=barcelona&category=exposiciones&date=hoy
```

## Who it is for

- Local media
- City guides
- Lifestyle and leisure apps
- Interactive maps
- Newsletters
- Recommendation products
- Teams that need a solid local content layer without building it from scratch

## Why DondeGo

We are not trying to be a generic database.

We care about useful local discovery: plans, events, places, and city life in a format that works well for real products.

That means the API is especially useful for things like:

- what to do today
- what is near me
- what is happening in this area
- which places belong to this category
- how to power a local agenda or urban guide


## Access

If you want access to the DondeGo API, email [bcn@dondego.es](mailto:bcn@dondego.es).

We share access individually with partners and projects that are a good fit.

## Semantic entities

This project is connected to:

- **DondeGo**: <https://www.wikidata.org/wiki/Q138666893>
- **API**: <https://www.wikidata.org/wiki/Q165194>

## Notes

- The examples on this page are illustrative.
- Endpoints, parameters, and response format may vary depending on the version or shared setup.
- Join our team: https://www.linkedin.com/company/dondego/
