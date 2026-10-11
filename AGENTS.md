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

## Transcribing voice notes

Recipes often arrive as rough speech-to-text transcripts.

1. Keep the speaker's wording and voice ("a ton of garlic", "squish them"); keep profanity, drop filler words ("like", "I don't know"), and break the rambling into stages.
2. Fix obvious transcription errors only when the meaning is clear from context (e.g. "610 cloves" → "6–10 cloves", "turn it on too" → "turn the burner to 2"). Burner numbers refer to the dial on the home stove.
3. Don't invent amounts, ingredients, or steps the note doesn't give. Leave them vague or blank.
4. Set `status: draft  # transcribed from a voice note`.
5. In Notes, list each guess with what was actually transcribed, plus anything missing.
6. In your reply, give the user a numbered list of questions (guesses to confirm, then missing details) so they can answer by number. As answers come in, update the recipe and remove resolved guesses from Notes; move anything left unresolved into an "Open question" note.
7. Don't commit until the user says to.

## Writing style

- Keep the family's voice and household-specific details (which pot, where an ingredient is kept). These are the point of the collection; don't genericize them.
- Note uncertainty honestly (e.g., "oven temp not confirmed") instead of inventing precision.
- Don't change quantities or steps unless asked.
