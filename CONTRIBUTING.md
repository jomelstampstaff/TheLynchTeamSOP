# Contributing to The Lynch Team SOP

You do **not** need to install anything to make edits. Every page on the live
site has a **pencil icon** in the top-right corner.

## Editing an Existing SOP

1. Go to the live SOP page.
2. Click the **pencil icon** (top-right).
3. GitHub opens an editor. Make your changes.
4. Scroll down, describe what you changed, click **"Create a new branch and start a pull request"**.
5. A teammate reviews and merges.
6. The site updates automatically in about 1 minute.

## Adding a New SOP

1. In the repo, go to `docs/`.
2. Click **Add file -> Create new file**.
3. Name it like `your-sop-name.md` (lowercase, hyphens).
4. Copy the contents of `docs/templates/sop-template.md` as a starting point.
5. Fill it in.
6. Open `mkdocs.yml`, find the `nav:` section, and add one line under the right category:

   ```yaml
   - Your SOP Name: your-sop-name.md
   ```

7. Commit both changes together.

## Writing Tips

- Use `#` for titles, `##` for sections, `###` for sub-sections.
- Use `-` for bullet lists and `1.` for numbered steps.
- Wrap warnings like this:

  ```
  !!! warning "Title"
      Your warning text here.
  ```

- Use `- [ ]` for checkboxes.
- Never use em dashes or long hyphens, use commas, periods, or parentheses.

## Need Help?

Ping @jomelstampstaff.
