---
title: 'queryCommandSupported'
attributions:
  - 'Microsoft Developer Network: [[queryCommandSupported Method](http://msdn.microsoft.com/en-us/library/ie/ms536681(v=vs.85).aspx) Article]'
notes:
  - 'Require manual conversion! See https://github.com/webplatform/mediawiki-conversion/issues/24'
readiness: 'Ready to Use'
relationships:
  method_of:
    predicate: 'Method of '
    value: dom/TextRange
    href: /dom/TextRange
  return_type:
    predicate: 'Returns an object of type  '
    value: Boolean
    href: /dom/TextRange
standardization_status: Non-Standard
summary: 'Returns a Boolean value that indicates whether the current command is supported on the current range.'
tags:
  - API_Object_Methods
  - DOM
uri: dom/TextRange/queryCommandSupported

---
<p>
</p>
<h2>Summary</h2>
<p>
Returns a Boolean value that indicates whether the current command is supported on the current range.</p><p>Method of <a href="/dom/TextRange">dom/TextRange</a><a href="/dom/TextRange">dom/TextRange</a>
</p>
<h2>Syntax</h2>
<pre class="js">
var result = document.queryCommandSupported(/* see parameter list */);
</pre>
<h2>Parameters</h2>
<h3>cmdID</h3>
<dl><dt> Data-type</dt>
<dd> BSTR</dd></dl><p><br/><b>String</b> that specifies a command identifier.
</p>
<h2>Return Value</h2>
<p>Returns an object of type  BooleanBoolean
</p><p>Boolean
</p><p><b>Boolean</b> that returns one of the following possible values:
</p>
<table class="wikitable"><tr><th>Return value
</th>
<th>Description
</th></tr><tr><td>true
</td>
<td>The command is supported.
</td></tr><tr><td>false
</td>
<td>The command is not supported.
</td></tr></table><p> 
</p>
<h2>Examples</h2>
<p>The follow example uses window.getSelection feature testing and if it is not supported by the client browser falls back to document.selection. 'queryCommandSupported' is then used on the range object to determine if the 'bold' command is supported in the current context.
</p>
<div class="example">
<pre class="js">
function makeBold(el){
if(window.getSelection){
	var sel=document.getSelection();
	var range = sel.getRangeAt(0),
  	content = range.extractContents(),
    span = document.createElement('b');
	span.appendChild(content);
	var htmlContent = span.innerHTML;
	range.insertNode(span);
}else{
	var sel=document.selection;
	if(sel){
		var rng=sel.createRange();
		if(rng.queryCommandSupported('bold')){
			if(rng.queryCommandEnabled('bold')){rng.execCommand('bold',false,null);}
		}
	}	
}

</pre>
<p><br/></p>
</div>
<h2>Usage</h2>
<pre> Used to add HTML markup to web documents.
</pre>
<h2>Notes</h2>
<h3>Remarks</h3>
<p>This method is a wrapper function for the command constants. You can obtain an <b>IHTMLDocument2</b> interface using IID_IHTMLDocument2 for the IID.
This method is a wrapper function for the command constants. You can obtain an <b>IHTMLControlRange</b> interface using IID_IHTMLControlRange for the IID.
This method is a wrapper function for the command constants. You can obtain an <b>IHTMLTxtRange</b> interface using IID_IHTMLTxtRange for the IID.
</p>
