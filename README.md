# Svggloo

Svggloo is a tool to perform a data-merge operation in an SVG file.

## Quickstart

The tool expects the following inputs:

- an SVG file to use as a template (see template details in the dedicated
  section below)
- a data file with the same name as the template, but with a `.csv` extension.
  Each record in the data file will produce a new output.

Usage:

```bash
svggloo --field country --field state --field city --export examples/quantifier/bike_lane_categories.svg
```

## Specifics

### Template

The template use the jinja2 syntax to perform replacements, therefore all
variables in the template must be surrounded by `{{}}`, for instance `{{name}}`.

### Data file

The data file must be a CSV file.
