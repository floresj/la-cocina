# Agent Guide: La Cocina

A family recipe collection. One markdown file per recipe. No code, no build.

## Layout

- `recipes/<category>/<recipe-name>.md` — categories: `mains`, `sides`, `soups-stews`, `breakfast`, `desserts`, `drinks`, `sauces-staples`. Create a category folder only when its first recipe is added.
- `templates/recipe-template.md` — the format every recipe must follow.
- `README.md` — the main page; its **Recipes** section links to every recipe.

## Adding or editing a recipe

1. Copy the template into the right category folder. Filename: lowercase, hyphens, no accents (`arroz-con-pollo.md`).
2. Fill in the front matter:
   - Times use `20m`, `1h30m`, `5h`.
   - `status: draft` until the recipe has been cooked and confirmed; then `tested`.
   - `added` is today's date (`YYYY-MM-DD`).
   - Leave a field blank rather than guessing. If you estimate a value, say so in your reply.
   - Do not add a `category` field; the folder is the category.
3. Sections: Ingredients and Equipment are bullet lists; Steps is a numbered list, each starting with a **bold stage label**; Notes is a bullet list.
4. **Update the Recipes section in `README.md`**: add a link under the right category heading, keep entries alphabetical, and add the heading if it's missing (headings in the category order above).

## Writing style

- Keep the family's voice and household-specific details (which pot, where an ingredient is kept). These are the point of the collection; don't genericize them.
- Note uncertainty honestly (e.g., "oven temp not confirmed") instead of inventing precision.
- Don't change quantities or steps unless asked.
