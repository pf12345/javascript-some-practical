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

2、element window height and width(100% height or width):

<pre>
1vw = 1% of viewport width

1vh = 1% of viewport height

1vmin = 1vw or 1vh, whichever is smaller

1vmax = 1vw or 1vh, whichever is larger

</pre>


<pre>
<code>
css style code:

div {
    height: 100vh;
	width: 100vw;
}

</code>
</pre>


3、chrome input autocomplete color change:

<pre>
input:-webkit-autofill, 
textarea:-webkit-autofill{
    -webkit-box-shadow: 0 0 0px 1000px #fff inset;
}
</pre>

4、chrome scoll bar style change:

<pre>
::-webkit-scrollbar-track-piece {
    background-color: #fff;
    -webkit-border-radius: 10px;
  }
  ::-webkit-scrollbar-thumb {
    background-color: #ecedf0;
    -webkit-border-radius: 10px;
    border: 1px solid #ecedf0;
  }
  ::-webkit-scrollbar {
    width: 10px;
    height: 10px;
  }

</pre>

5、在定高div中放置一个img图片(大小不定)的上下居中方式：

<pre>
(1)
&lt;div class='frame'&gt;
    &lt;img src="" alt="" /&gt;
&lt/div&gt;
&lt;style&gt;
   .frame {
      height: 300px;
      width: 300px;
      position: relative;
   }

   .frame img {
      postion: absolute;
      top: 0;
      bottom: 0;
      right: 0;
      left: 0;
      margin: auto;
      max-height: 280px;
      max-width: 280px;
   }

&lt;/style&gt;

(2)
&lt;div class='frame'&gt;
    &lt;div&gt;
        &lt;img src="" alt="" /&gt;
    &lt;/div/&gt;
&lt/div&gt;
&lt;style&gt;
   .frame {
      height: 300px;
      width: 300px;
      position: relative;
      display: table;
   }
   .frame > div {
      display: table-cell;
      vertical-align: middle;
   }

   .frame img {
      max-height: 280px;
      max-width: 280px;
   }

&lt;/style&gt;
</pre>