---
sidebar_position: 0
---

# Config API

The PTRUI Framework allows for App UI customizations through the `Config.tsx` file that is included in the PTRUI Template Repo.

## Meta

### Name

App name.

```ts
config.setName(name: string)
```

### Version

App version number.

```ts
config.setVersion(version: string | number | JSX.Element)
```

### Logo Type

Allows for App Logo to be chosen.

```ts
config.setLogoType(type: 'optimiz' | 'protrans)
```

## Layout

### Language Switcher

Enables language switcher icon and dropdown in App header

```ts
config.enableLanguageSwitcher(isEnabled: boolean)
```

### Global Search

Enables global search icon and input in the App header

```ts
config.enableGlobalSearch(isEnabled: boolean)
```

### Auto Collapse Sidebar

Auto collapses sidebar on specified pages. Passing `true` will collapse the sidebar on all pages by default.

```ts
config.setSideBarCollapsePaths(path: string[] | boolean)
```

### Hide Sidebar

Hides Sidebar on specified pages. Passing `true` will hide the sidebar on all pages by default.

```ts
config.sideBarHidePaths(path: string[] | boolean)
```

## SSO

### Client ID

Sets App specific Client ID that is needed for SSO.

```ts
config.setClientId(clientID: string)
```

### No Auth Redirect URL

Redirects App to external login URL if not authenticated.

```ts
config.setRedirectURL(redirectUrl: string)
```

### Logout Redirect URL

Redirects App to external login URL if not authenticated.

```ts
config.setLogoutRedirectURL(url: string)
```

### Disable SSO Login

Disables the SSO Login.

```ts
config.disableSSOLogin(disable: boolean)
```

## Global Fetch Credentials

### Fetch Profiles

Create multiple global fetch credential profiles to be used by the `useFetch` hook.

```ts
config.setFetchProfiles<R = Response>(profiles: { [key: string]: IProfileOptions<R>; default: IProfileOptions<R>; })
```
