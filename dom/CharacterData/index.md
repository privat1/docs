---
title: 'CharacterData'
readiness: 'Ready to Use'
relationships:
  subclass_of:
    predicate: 'Inherits from '
    value: Node
    href: /dom/Node
standardization_status: 'W3C Recommendation'
summary: 'An interface for accessing character data and performing common character data operations for objects in the DOM.'
tags:
  - API_Objects
  - DOM
uri: dom/CharacterData

---
## Summary

An interface for accessing character data and performing common character data operations for objects in the DOM.

Inherits from [Node](/dom/Node)[Node](/dom/Node)

## Properties

[html/elements/data](/dom/CharacterData/data)
:   Sets or gets a node's character data.

[length](/dom/CharacterData/length)
:   Gets the number of characters in a text node.

## Methods

[appendData](/dom/CharacterData/appendData)
:   Appends a string to the end of the character data.

[deleteData](/dom/CharacterData/deleteData)
:   Removes a specified range of characters from the node.

[insertData](/dom/CharacterData/insertData)
:   Inserts a new character string into the node at the specified offset.

[replaceData](/dom/CharacterData/replaceData)
:   Replaces a specified range of characters in the node with a new character string.

[substringData](/dom/CharacterData/substringData)
:   Extracts a range of characters from the node.

## Events

*No events.*

## Inherited from Node

### Properties

[attributes](/dom/Node/attributes)
:   Associatve array containing the attributes of node.

[childNodes](/dom/Node/childNodes)
:   Gets a collection of direct Node descendants of the Node, including [Element](/dom/Element), [Text](/dom/Text) and any other type of nodes.

[firstChild](/dom/Node/firstChild)
:   Gets a reference to the first child node in the childNodes collection of the object.

    If the node is childless, null is returned.

[lastChild](/dom/Node/lastChild)
:   Gets a reference to the last child in the childNodes collection of an object.

[localName](/dom/Node/localName)
:   Retrieves the local name of the fully qualified XML declaration for a node.

[namespaceURI](/dom/Node/namespaceURI)
:   Retrieves the namespace URI of the fully qualified XML declaration for a node.

[nextSibling](/dom/Node/nextSibling)
:   Retrieves the next child node of the parent of the node.

[nodeName](/dom/Node/nodeName)
:   Gets the name of a particular type of node.

[nodeType](/dom/Node/nodeType)
:   Retrieves the type of the requested node.

[nodeValue](/dom/Node/nodeValue)
:   Gets or sets the value of a Node, if the type of Node supports it.

[ownerDocument](/dom/Node/ownerDocument)
:   Retrieves the document object associated with the node.

[parentNode](/dom/Node/parentNode)
:   Retrieves the parent node in the document hierarchy.

[prefix](/dom/Node/prefix)
:   Sets or retrieves the prefix of the fully qualified XML declaration for a node.

[previousSibling](/dom/Node/previousSibling)
:   Retrieves the previous child node of the parent of the node.

[textContent](/dom/Node/textContent)
:   Sets or retrieves the text content of a node and any child nodes.

### Methods

[appendChild](/dom/Node/appendChild)
:   Appends an element as a child to the object.

[cloneNode](/dom/Node/cloneNode)
:   Copies a reference to the object from the document hierarchy.

[compareDocumentPosition](/dom/Node/compareDocumentPosition)
:   Compares the position of two nodes in a document.

[empty](/dom/Node/empty)
:   Cancels the current selection, sets the selection type to none, and sets the item property to null.

[hasAttributes](/dom/Node/hasAttributes)
:   Returns whether this node (if it is an element) has any attributes

[hasChildNodes](/dom/Node/hasChildNodes)
:   Gets a value that indicates whether the Node has any direct Node descendant of any type.

[insertBefore](/dom/Node/insertBefore)
:   Inserts a child into the node, immediately before the specified reference child node.

[isDefaultNamespace](/dom/Node/isDefaultNamespace)
:   Indicates whether or not a namespace is the default namespace for a document.

[isEqualNode](/dom/Node/isEqualNode)
:   Determines whether two nodes are equal in their type, name and namespace.

[isSameNode](/dom/Node/isSameNode)
:   Determines if two nodes are the same node.

[isSupported](/dom/Node/isSupported)
:   Returns a value indicating whether or not the object supports a specific DOM standard.

[lookupNamespaceURI](/dom/Node/lookupNamespaceURI)
:   Gets the URI of the namespace associated with a namespace prefix, if any.

[lookupPrefix](/dom/Node/lookupPrefix)
:   Gets the namespace prefix associated with a URI, if any.

[normalize](/dom/Node/normalize)
:   Merges adjacent DOM objects to produce a normalized document object model.

[removeChild](/dom/Node/removeChild)
:   Removes a child node from a node.

[replaceChild](/dom/Node/replaceChild)
:   Replaces an existing child node with a new child node.

### Events

*No events.*

## Inherited from EventTarget

### Properties

*No properties.*

### Methods

[addEventListener](/dom/EventTarget/addEventListener)
:   Registers an event handler for the specified event type.

[dispatchEvent](/dom/EventTarget/dispatchEvent)
:   Sends an event to the current element.

[removeEventListener](/dom/EventTarget/removeEventListener)
:   Removes an event handler that the [addEventListener](/dom/EventTarget/addEventListener) method registered.

### Events

*No events.*

## Related specifications

[DOM Level 3 Core](http://www.w3.org/TR/DOM-Level-3-Core/)
:   Recommendation
