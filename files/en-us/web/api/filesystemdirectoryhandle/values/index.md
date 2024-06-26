---
title: "FileSystemDirectoryHandle: values() method"
short-title: values()
slug: Web/API/FileSystemDirectoryHandle/values
page-type: web-api-instance-method
browser-compat: api.FileSystemDirectoryHandle.values
---

{{securecontext_header}}{{APIRef("File System API")}}

The **`values()`** method of the
{{domxref("FileSystemDirectoryHandle")}} interface returns a new _array iterator_
containing the values for each index in the `FileSystemDirectoryHandle`
object.

## Syntax

```js-nolint
values()
```

### Parameters

None.

### Return value

A new {{jsxref('Array')}}

## Examples

```js
const dirHandle = await window.showDirectoryPicker();

for await (const value of dirHandle.values()) {
  console.log(value);
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [File System API](/en-US/docs/Web/API/File_System_API)
- [The File System Access API: simplifying access to local files](https://developer.chrome.com/articles/file-system-access/)
