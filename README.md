# OpenCocktail Library

A collection of cocktail recipes using the [OpenCocktail](./schema.json) recipe format base off of Techhat's [Open Recipe Format](https://github.com/techhat/openrecipeformat).

## Prerequisites

You will need to know a few cocktail recipes. If you don't know any, well, you've come to the right place.

* [View recipe files](./recipes/)

## Contributing

### Coding

First, [install Pre-commit](https://pre-commit.com/#install). Once pre-commit is installed, in the project root directory run:

```bash
pre-commit install
```

When you make a commit the following hooks will run against your changes:

* Check for trailing whitespace
* YAML formatting
* JSON schema checking

The first two will make changes to your files if needed and you will need to run your commit again in order for those changes to take. If you have schema errors you will need to correct those before and run your commit until they are fixed.

### Creating

Create recipes using the schema outline in the [schema.json](./schema.json) file. Add new recipes to the [recipes](./recipes/) directory. The basic format is as follows:

```yaml
---
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
  - step: Add gin to a collins glass.
  - step: Add tonic water.
source_book:
  authors:
  - Some Person
  title: Gin and Tonic for Dummies
  isbn: '1234567890'
```

### Git workflow

* Create a new branch
* Add your code
* Commit and pass the pre-commits
* Push your code and create a pull request

## Testing

Mix one or more of the cocktails and then test them.

## Authors

* Tom Camp - [Tom-Camp](https://github.com/Tom-Camp)

## License

This project is licensed under [CC0 1.0 Universal](./LICENSE)
