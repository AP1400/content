---
title: "FileSystemDirectoryHandle: entries() method"
short-title: entries()
slug: Web/API/FileSystemDirectoryHandle/entries
page-type: web-api-instance-method
browser-compat: api.FileSystemDirectoryHandle.entries
---

{{securecontext_header}}{{APIRef("File System API")}}

The **`entries()`** method of the
{{domxref("FileSystemDirectoryHandle")}} interface returns an array of a given object's
own enumerable property `[key, value]` pairs, in the same order as that
provided by a [`for...in`](/en-US/docs/Web/JavaScript/Reference/Statements/for...in) loop (the difference being that a for-in loop
enumerates properties in the prototype chain as well).

## Syntax

```js-nolint
entries()
```

### Parameters

None.

### Return value

An array of the given `FileSystemDirectoryHandle` object's own enumerable
property `[key, value]` pairs.

## Examples

```js
const dirHandle = await window.showDirectoryPicker();

for await (const [key, value] of dirHandle.entries()) {
  console.log({ key, value });
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [File System API](/en-US/docs/Web/API/File_System_API)
- [The File System Access API: simplifying access to local files](https://developer.chrome.com/articles/file-system-access/)
