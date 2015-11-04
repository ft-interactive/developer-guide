# Naming conventions

## Format for filenames and directory names

Basic rules:

- All lowercase.
- Use hyphens to separate words (not camelCase, and no_underscores_please)
- Don't include dates or any technical metadata unless you have a very good reason.
- Just name it what it is, being clear and precise (`david-cameron.jpg` is beter than `photo.jpg`).
- Avoid abbreviating things too much. Filenames don't need to be short.
- Never put things like `-new` or `-fixed` or `-FINAL` in a filename. Instead, just replace the old file, keeping the name the same, and track the change with git – this is usually better than having multiple versions of a file knocking about. If you *really* need to version a filename, just append it with a number (e.g. `cat-2`), then at least you can increment the number later if necessary.
