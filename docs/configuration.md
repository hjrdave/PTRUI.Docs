---
sidebar_position: 2
---

# Configuration

The PTRUI Framework allows for App UI customizations through the `Config.tsx` file that is included in the PTRUI Template Repo.

## Config API

### Name

App name.

```js
config.setName(name: string)
```

### Version

App version number.

```js
config.setVersion(version: string | number | JSX.Element)
```

### Logo Type

Allows for App Logo to be chosen.

```js
config.setLogoType(type: 'optimiz' | 'protrans)
```

### Language Switcher

Enables language switcher icon and dropdown in App header

```json
config.enableLanguageSwitcher(isEnabled: boolean)
```
