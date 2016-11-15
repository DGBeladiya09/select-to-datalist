# select-to-datalist
Script to convert select boxes to inputs with associated datalists


## Expected Markup Pattern:

```html
<label for="ex_1" data-action="prog-datalist">
  <span class="label__text">
    Label:
  </span>
  <span class="select-box"> <!-- optional -->
    <select id="ex_1" name="ex_1">
      <option disabled selected>Select:</option>
      <option>...</option>
    </select>
  </span> <!-- /optional -->
</label>
```
