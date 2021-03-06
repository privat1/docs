---
title: 'replaceWholeText'
attributions:
  - 'Mozilla Developer Network [![cc-by-sa-small-wpd.svg](/assets/thumb/8/8c/cc-by-sa-small-wpd.svg/120px-cc-by-sa-small-wpd.svg.png)](http://creativecommons.org/licenses/by-sa/3.0/us/): [[Text.replaceWholeText](https://developer.mozilla.org/en-US/docs/Web/API/Text.replaceWholeText) Article]'
  - 'Microsoft Developer Network: [[replaceWholeText Method](http://msdn.microsoft.com/en-us/library/ie/ff975208(v=vs.85).aspx) Article]'
notes:
  - "Needs example....\nleave for me..."
readiness: 'Almost Ready'
relationships:
  method_of:
    predicate: 'Method of '
    value: dom/Text
    href: /dom/Text
  return_type:
    predicate: 'Returns an object of type  '
    value: 'DOM Node'
    href: /dom/Text
standardization_status: Deprecated
summary: 'Replaces the text of the current object.'
tags:
  - API_Object_Methods
  - DOM
  - Needs_Examples
uri: dom/Text/replaceWholeText

---
## Summary

Replaces the text of the current object.

Method of [dom/Text](/dom/Text)[dom/Text](/dom/Text)

## Syntax

``` js
var textNode = textNode.replaceWholeText(/* see parameter list */);
```

## Parameters

### text

 Data-type
:   String

 The text that replaces the existing text.

## Return Value

Returns an object of type DOM NodeDOM Node

A [**Text**](/dom/Text) node that received the replacement text. If the replaced text was empty, this value will be null. If the current node is read-only, a new **Text** node is returned. If the current node is not read-only, the same object is returned.

## Notes

Obsolete

This feature is obsolete. Although it may still work in some browsers, its use is discouraged since it could be removed at any time. Try to avoid using it.

## Related specifications

[DOM Level 3 Core](http://www.w3.org/TR/DOM-Level-3-Core/)
:   Recommendation

[DOM](http://dom.spec.whatwg.org/#text)
:   Living Standard
