1、popup
<pre>
<code>
html code:

&lt;div class="modal-popup">
    &lt;div class="arrow">&lt/div>
    &lt;div class="content">
        on the left
    &lt;/div>
&lt;/div>
</code>
</pre>

<pre>
<code>
css style code:

.arrow,
.arrow:after {
    position: absolute;
    display: block;
    width: 0;
    height: 0;
    border-color: transparent;
    border-style: solid;
}
.arrow {
    border-width: 6px;
}
.arrow {
    top: 50%;
    right: -6px;
    margin-top: -6px;
    border-right-width: 0;
    border-left-color: #ffdc51;
}
.arrow:after {
    border-width: 10px;
    content: "";
}
.arrow:after {
    content: " ";
    right: 1px;
    border-right-width: 0;
    border-left-color: #ffdc51;
    bottom: -10px;
}
.modal-popup {
    position: relative;
    display: inline-block;
}
.content {
    background-color: #ffdc51;
    padding: 6px 10px;
     border-radius: 2px;
}
</code>
</pre>