# Conventional Commit Builder for Vint

Use the `commit` function from the `actions` package to interactively build a conventional commit message. The tool prompts you for:

- **Type:** (e.g., feat, fix, docs, etc.)
- **Scope:** (optional, e.g., authentication)
- **Description:** (required)
- **Body:** (optional)
- **Breaking Change:** (optional; if yes, provide details)
- **Issue Number:** (optional, e.g., 123 becomes "Closes #123")

After collecting your inputs, the commit preview is displayed. Confirm to run:

- `git add .`
- `git commit -m '<your commit message>'`
- `git push`

Example usage in Vint:

```vint
import actions
actions.commit()
```
