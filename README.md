```{bash}
quarto render index.qmd 
```

Fails with:

```
Executing 'embed.ipynb'
  Cell 1/1: 'two'...Done

ERROR: The cell two does not exist in notebook
```

Embed works if label if prefixed by `cell-`:
```
{{< embed embed.qmd#cell-two >}}
```