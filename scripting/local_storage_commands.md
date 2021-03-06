# Local Storage Commands

These commands allow you to access properties in local storage for the [origin](https://developer.mozilla.org/en-US/docs/Glossary/Origin) of the current page.

This document assumes you already have some knowledge about [local storage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage).

## List of commands
| Command | Description|
|---------|------------|
| [`UI.LocalStorage.get`](#uilocalstorageget) | Get the value of a property from local storage|
| [`UI.LocalStorage.set`](#uilocalstorageset) | Set a property in local storage |
| [`UI.LocalStorage.isSet`](#) | - coming soon - |
| [`UI.LocalStorage.isEqual`](#) | - coming soon - |
| [`UI.LocalStorage.delete`](#uilocalstoragedelete) | Delete a property in local storage |
| [`UI.LocalStorage.deleteAll`](#uilocalstoragedeleteall) | Delete all properties in local storage |

--- 

## `UI.LocalStorage.get`

Get the value of a property from local storage for the [origin](https://developer.mozilla.org/en-US/docs/Glossary/Origin) of the current page.

Returns `null` if the property does not exist.

If the property exists, its value will be automatically parsed as a JSON object if it is a valid JSON object, otherwise it will be returned as a string.

### Usage

```javascript
UI.LocalStorage.get(name)
```

| Parameter | Type | Remarks |
|-----------|------|---------|
| name | string | The name of the property to get from local storage |

### Example(s)

Here's how we can access the local storage in our test script to get the value of the `cart` property for example:
```javascript
var cart = UI.LocalStorage.get("cart")
```

--- 

## `UI.LocalStorage.set`

Set a property in local storage for the [origin](https://developer.mozilla.org/en-US/docs/Glossary/Origin) of the current page.

If the property already exists in local storage, the value is overriden.

### Usage

```javascript
UI.LocalStorage.set(name, value)
```

| Parameter | Type | Remarks |
|-----------|------|---------|
| name | string | The name of the property to put in local storage |
| value | any | The value to the property to put in local storage. If the value is not a string, it will be stringified before saving. |

### Example(s)

Set the `theme` property in local storage to `{"dark_mode": true}`: 
```javascript
UI.LocalStorage.set("theme", {"dark_mode": true})
```

--- 

## `UI.LocalStorage.delete`

Delete a property in local storage for the [origin](https://developer.mozilla.org/en-US/docs/Glossary/Origin) of the current page.

### Usage

```javascript
UI.LocalStorage.delete(name)
```

| Parameter | Type | Remarks |
|-----------|------|---------|
| name | string | The name of the property to delete from local storage |

### Example(s)

Delete the `cart` property from local storage:
```javascript
UI.LocalStorage.delete("cart")
```

--- 

## `UI.LocalStorage.deleteAll`

Delete all properties in local storage for the [origin](https://developer.mozilla.org/en-US/docs/Glossary/Origin) of the current page.

### Usage

```javascript
UI.LocalStorage.deleteAll()
```
