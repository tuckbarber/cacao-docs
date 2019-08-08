---
   id: layout
   title: Layout
---

<a class="sourceView-page" href="https://github.com/aptuitiv/cacao/blob/master/src/css/utils/layout/layout.css"></a>

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
    height: 400px;
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
.example-parent img{
    margin: 10px;
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
Using u-nbfc utility on container to contain floated children.
<div class="example-divider">
    <div class="example-parent u-nbfc">
            <!-- Photo by Hannah Busing on Unsplash -->
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150" class="u-floatLeft">
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                          &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150" class="u-floatRight">
            <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras nisi augue, facilisis vitae elit at, tincidunt semper lorem. Phasellus interdum aliquet vehicula. Praesent tristique lectus tellus, sed hendrerit leo consequat eget. In hac habitasse platea dictumst. Morbi ac scelerisque ipsum. Nullam id eros at mauris consequat laoreet.    
            </p>
    </div>
</div>

Using u-nbfc utility on container to contain floated children, and u-nbfc used on child &lt;p&gt; element to prevent its text from wrapping under floated elements.
<div class="example-divider">
    <div class="example-parent u-nbfc">
            <!-- Photo by Hannah Busing on Unsplash -->
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150" class="u-floatLeft">
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                          &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150" class="u-floatRight">
            <p class="u-nbfc">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras nisi augue, facilisis vitae elit at, tincidunt semper lorem. Phasellus interdum aliquet vehicula. Praesent tristique lectus tellus, sed hendrerit leo consequat eget. In hac habitasse platea dictumst. Morbi ac scelerisque ipsum. Nullam id eros at mauris consequat laoreet.    
            </p>
    </div>
</div>

</div>
