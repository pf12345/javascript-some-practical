1、popup
<pre>
<code>
html code:

&lt;div class="modal-popup">
    &lt;div class="arrow-left arrow">&lt/div>
    &lt;div class="content">
        on the left
    &lt;/div>
&lt;/div>

&lt;div class="modal-popup">
    &lt;div class="arrow-right arrow">&lt/div>
    &lt;div class="content">
        on the right
    &lt;/div>
&lt;/div>
</code>
</pre>

<pre>
<code>
css style code:

        .arrow,
        .arrow:after 
        {
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
            margin-top: -6px;
        }
        .arrow.arrow-right{
            border-right-width: 0;
            border-left-color: #ffdc51;
            right: -6px;
        }
        .arrow.arrow-left{
            border-left-width: 0;
            border-right-color: #ffdc51;
            left: -6px;
        }
        .arrow.arrow-bottom {
            border-bottom-width: 0;
            border-top-color: #ffdc51;
            top: 35px;
            left: 50%;
            margin-left: -6px;;
        }
        .arrow.arrow-top {
            border-top-width: 0;
            border-bottom-color: #ffdc51;
            top: 0;
            left: 50%;
            margin-left: -6px;;
        }
        .arrow:after {
            border-width: 10px;
            content: "";
        }
        .arrow:after {
            content: " ";
            bottom: -10px;
        }
        .arrow.arrow-right:after {
            border-right-width: 0;
            border-left-color: #ffdc51;
            right: 1px;
        }
        .arrow.arrow-left:after {
            border-left-width: 0;
            border-right-color: #ffdc51;
            left: 1px;
        }
        .arrow.arrow-bottom:after {
            border-bottom-width: 0;
            border-top-color: #ffdc51;
            top: -6px;
            left: -9px;
        }
        .arrow.arrow-bottom:after {
            border-top-width: 0;
            border-bottom-color: #ffdc51;
            top: -6px;
            left: -9px;
        }
        .modal-popup {
            position: relative;
            display: inline-block;
        }
        .content {
            background-color: #ffdc51;
            padding: 6px 10px;
            border-radius: 2px;
            color: #796100;
        }
</code>
</pre>

2、element window height(100% height):

<pre>
<code>
css style code:

div {
    height: 100vh;
}

</code>
</pre>