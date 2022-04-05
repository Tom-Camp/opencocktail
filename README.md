# OpenCocktail Library

A collection of cocktail recipes using the [OpenCocktail](./schema.json) recipe format base off
of Techhat's [Open Recipe Format](https://github.com/techhat/openrecipeformat).

## Prerequisites

You will need to know a few cocktail recipes. If you don't know any, well, you've
come to the right place. [View recipe files](./recipes/)

## Contributing

Create recipes using the schema outline in the [schema.json](./schema.json) file. Add
new recipes to the [recipes](./recipes/) directory. The basic format is as follows:

```yaml
drink_name: Gin & Tonic
ingredients:
  - gin:
    amounts:
      - amount: 2.5
        unit: ounce
  - tonic water:
    amounts:
      - amount: 4
        unit: ounce
drink_type: tonic
garnish: Garnish with a slice of lime.
serve_in: collins glass
steps:
  - step:
      Add gin to a collins glass.
  - step:
      Add tonic water.
```

## Testing

Mix one or more of the cocktails and then test them.

## Authors

* Tom Camp - [Tom-Camp](https://github.com/Tom-Camp)

## License

This project is licensed under [CC0 1.0 Universal](./LICENSE)
