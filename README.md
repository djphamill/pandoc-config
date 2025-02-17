# Pandoc Configuartion

Can set a template file as the default by overwritting the default.<FORMAT> tempalte. For example
```bash
sudo cp template.html /usr/share/pandoc/data/templates/default.html
```
writes a new default template for the HTML format.

To invoke the HTML template, pass the standalone `-s` flag:
```bash
pandoc -s path/to/input/file -o path/to/file.html --metadata title="My Title"
```
Some variables may _need_ to be defined for the tempalte, such as title for HTML.
