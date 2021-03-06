---
title: 'aria-controls'
attributions:
  - 'Microsoft Developer Network: [[Windows Internet Explorer API reference](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx) Article]'
compatibility:
  feature: aria-controls
  topic: aria
notes:
  - 'Needs summary, example, spec reference, standardization status'
readiness: 'Not Ready'
tags:
  - Markup_Attributes
  - Accessibility
  - ARIA
  - Needs_Summary
  - Needs_Examples
uri: aria/attributes/aria-controls

---
<table class="wikitable">
<tr>
<th>
Applies to

</th>
<td>
</td>
</tr>
</table>
## Notes

### Remarks

<table class="wikitable">
<tr>
<th>
Used in Roles

</th>
<td>
<dl>

<dt>
No role required.

</dt>
</dl>
</td>
</tr>
</table>
  This property defines element relationships and associations that cannot be readily determined from the document structure. The **aria-controls** property is used primarily by elements where the [**role**](/html/attributes/role) property value is `group`, `region`, or `widget`. Compare this usage with that of the [**aria-owns**](/aria/attributes/aria-owns) property. **Note**  For cross-browser compatibility, always use the WAI-ARIA attribute syntax to access and modify ARIA properties, for example `object.setAttribute("aria-valuenow", newValue)`.

### Syntax

### Standards information

-   [Accessible Rich Internet Applications (WAI-ARIA) 1.0](http://go.microsoft.com/fwlink/p/?linkid=203793), Section 6.6

## See also

### Related pages

-   Accessible Rich Internet Applications (ARIA)[Accessible Rich Internet Applications (ARIA)](/aria)
-   `Reference`
-   aria-describedby[aria-describedby](/aria/attributes/aria-describedby)
-   aria-flowto[aria-flowto](/aria/attributes/aria-flowto)
-   aria-labelledby[aria-labelledby](/aria/attributes/aria-labelledby)
-   aria-owns[aria-owns](/aria/attributes/aria-owns)
-   aria-posinset[aria-posinset](/aria/attributes/aria-posinset)
-   aria-setsize[aria-setsize](/aria/attributes/aria-setsize)
