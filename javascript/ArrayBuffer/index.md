---
title: 'ArrayBuffer'
attributions:
  - 'Microsoft Developer Network: [Article](http://msdn.microsoft.com/en-us/library/ie/br212474(v=vs.94).aspx)'
compatibility:
  feature: ArrayBuffer
  topic: javascript
readiness: 'Ready to Use'
summary: "Represents a raw buffer of binary data, which is used to store data for the different typed arrays. ArrayBuffers cannot be read from or written to directly, but can be passed to a typed array or DataView Object to interpret the raw buffer as needed.\n"
tags:
  - JS_Basic
uri: javascript/ArrayBuffer

---
## Summary

Represents a raw buffer of binary data, which is used to store data for the different typed arrays. ArrayBuffers cannot be read from or written to directly, but can be passed to a typed array or DataView Object to interpret the raw buffer as needed.

For more information about typed arrays, see Typed Arrays.

## Syntax

    arrayBuffer = new ArrayBuffer(length);

**arrayBuffer**
:   Required. The variable name to which the **ArrayBuffer** object is assigned.

**length**
:   The length of the buffer. The contents of the ArrayBuffer are initialized to 0. If the requested number of bytes could not be allocated an exception is raised.

## Examples

The following example shows how to use an ArrayBuffer object to process the binary data acquired from an XmlHttpRequest. You can use a [DataView Object](/javascript/DataView) to get the individual values.

``` js
var req = new XMLHttpRequest();
     req.open('GET', "http://www.example.com");
     req.responseType = "arraybuffer";
     req.send();

     req.onreadystatechange = function () {
         if (req.readyState === 4) {
             var buffer = req.response;
             var dataview = new DataView(buffer);
             var ints = new Int32Array(buffer.byteLength / 4);
             for (var i = 0; i < ints.length; i++) {
                 ints[i] = dataview.getInt32(i * 4);
             }
         alert(ints[10]);
         }
     }
```

## Remarks

For more information about using XmlHttpRequest , see XMLHttpRequest enhancements.

## Properties

The following table lists the properties of the **ArrayBuffer** object.

|Property|Description|
|:-------|:----------|
|[byteLength](/javascript/ArrayBuffer/byteLength)|Read-only. The length of the ArrayBuffer (in bytes).|

