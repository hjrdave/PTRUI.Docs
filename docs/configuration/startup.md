---
sidebar_position: 1
---

# Start Up Scripts

React scripts can be added to the `Startup.tsx` file in the PTRUI Template. These scripts are global and will run as soon as the App loads.

The example below shows a script that handles language switching.

```ts
import React from 'react';
import PTRUI from 'protrans-react-ui';
import useI18N from './hooks/use-i18n';

export default function StartUp() {

    const { fetchLocalizeData, localeKey } = useI18N();

    //updates localize data
    PTRUI.useNonInitialEffect(() => {
        fetchLocalizeData(localeKey);
    }, [localeKey]);


    return null;
}
```
