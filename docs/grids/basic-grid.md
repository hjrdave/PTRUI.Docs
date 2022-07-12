---
sidebar_position: 2
---

# Basic Grid

Basic data grid with pagination, export features, and internal state management.

```jsx
<BasicGrid data={[]}>
    <BasicGrid.Header>
        {/*Filter controls and components that need access to Grid state*/}
    </BasicGrid.Header>
    <BasicGrid.UtilBar>
        <div className='d-flex justify-content-between w-100'>
            <div>
                <BasicGrid.ExportToPDF className={'mr-2'} />
                <BasicGrid.ExportToExcel className={'mr-2'} />
                <BasicGrid.RefreshData />
            </div>
        </div>
    </BasicGrid.UtilBar>
    <BasicGrid.Table>
        <BasicGrid.Column
            field={'id'}
            title={'ID'}
        />
        <BasicGrid.Column
            field={'name'}
            title={'Name'}
        />
        <BasicGrid.Column
            field={'description'}
            title={'Description'}
        />
    </BasicGrid.Table>
    <BasicGrid.Footer>
        <div className='d-flex justify-content-end'>
            <BasicGrid.Counter />
        </div>
    </BasicGrid.Footer>
</BasicGrid>
```

## Props

### `BasicGrid`

```jsx
import {BasicGrid} from 'protrans-react-ui'
```

| Name | Type | Default | Description |
| ----------- | ----------- | ----------- | ----------- |
| name | type | default | description |

### `BasicGrid.Header`

| Name | Type | Default | Description |
| ----------- | ----------- | ----------- | ----------- |
| name | type | default | description |

### `BasicGrid.UtilBar`

| Name | Type | Default | Description |
| ----------- | ----------- | ----------- | ----------- |
| name | type | default | description |

### `BasicGrid.Table`

| Name | Type | Default | Description |
| ----------- | ----------- | ----------- | ----------- |
| name | type | default | description |

### `BasicGrid.Column`

| Name | Type | Default | Description |
| ----------- | ----------- | ----------- | ----------- |
| name | type | default | description |

### `BasicGrid.Footer`

| Name | Type | Default | Description |
| ----------- | ----------- | ----------- | ----------- |
| name | type | default | description |
