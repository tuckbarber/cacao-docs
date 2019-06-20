---
   id: layout
   title: Layout
---

To help with layout bugs and tricks.

## Available classes

* `u-cf`: Applies a clearfix to prevent an element that contains float elements from collapsing.
* `u-floatLeft`: Float an element to the left.
* `u-floatRight`: Float an element to the right.
* `u-nbfc`: Adds a 'new block formatting context', won't let element wrap under floats and
contains all floated children. Will clip overflowing content.
* `u-nbfcAlt`: An alternative to `u-nbfc` that avoids clipping overflow content.

## Usage


<style>
.example-divider{
    margin-bottom: 300px;
}
.example-divider:last-child{
    margin-bottom: 0;
}
.example-parent{
    border: 2px #bbb dashed;
    display:block;
    margin: 20px auto;
    padding: 10px;
    width: 80%;
}
</style>

<div class="code-sample">
<br>
Without using u-cf utility on container of floated content.
<div class="example-divider">
    <div class="example-parent">
            <!-- Photo by Hannah Busing on Unsplash -->
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150" class="u-floatLeft">
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                          &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150" class="u-floatRight">
    </div>
</div>
Using u-cf utility on container to keep it from collapsing.
<div class="example-divider">
    <div class="example-parent u-cf">
            <!-- Photo by Hannah Busing on Unsplash -->
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150" class="u-floatLeft">
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                          &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150" class="u-floatRight">
    </div>
</div>
</div>
