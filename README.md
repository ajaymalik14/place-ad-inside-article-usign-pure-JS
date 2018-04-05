# place-ad-inside-article-usign-pure-JS
<div id=ad'>Ad Content</div>
           <div id='con'></div>
<pre>
function insertAfter(addition,target) {
var parent = target.parentNode;
if (parent.lastChild == target) {
parent.appendChild(addition);
} else {
parent.insertBefore(addition,target.nextSibling);
}
}
var adscont = document.getElementById(&quot;ads&quot;);
var target = document.querySelectorAll(&quot;article&quot;);
var linebreak = target[0].getElementsByTagName(&quot;p&quot;);
if (linebreak.length &gt; 0){
insertAfter(adscont,linebreak[5]);
}
</pre>
