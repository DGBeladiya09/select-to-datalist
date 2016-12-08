# Select Bot to Datalist Script

Vanilla JavaScript to convert select boxes to inputs with associated datalists.


## What does it do?

The script will go through your document and find instances of ```data-action="prog-datalist"``` and convert the following pattern from:

```html
<label for="ex_1" data-action="prog-datalist" data-class="text-input">
  <span class="label__text">
    Label Text:
  </span>
  <!-- <span class="select-box"> -->
    <select id="ex_1" name="ex_1" required>
      <option disabled selected>Select:</option>
      <option>option 1</option>
      <option>option 2</option>
      <option>option 3</option>
    </select>
  <!-- </span> -->
</label>
```   

to   

```html
<label for="ex_1" data-action="prog-datalist">
  <span class="label__text">
    Label Text:
  </span>
  <input type="text"
    id="ex_1" 
    name="ex_1" 
    required 
    list="datalist_2121" 
    class="text-input">
  <datalist id="datalist_2121">
    <option>option 1</option>
    <option>option 2</option>
    <option>option 3</option>
  </datalist>
</label>
```
  
