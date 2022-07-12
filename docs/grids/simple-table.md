---
sidebar_position: 1
---

# Simple Table

Simple table component that can be used to show data in a tabular layout.

```jsx
<Table>
    <Table.Head>
        <Table.Column>#</Table.Column>
        <Table.Column>First Name</Table.Column>
        <Table.Column>Last Name</Table.Column>
        <Table.Column>Username</Table.Column>
    </Table.Head>
    <Table.Body>
        <Table.Row>
            <Table.Cell>1</Table.Cell>
            <Table.Cell>Mark</Table.Cell>
            <Table.Cell>Otto</Table.Cell>
            <Table.Cell>mdo</Table.Cell>
        </Table.Row>
        <Table.Row>
            <Table.Cell>2</Table.Cell>
            <Table.Cell>Jacob</Table.Cell>
            <Table.Cell>Thornton</Table.Cell>
            <Table.Cell>fat</Table.Cell>
        </Table.Row>
        <Table.Row>
            <Table.Cell colSpan={4}>3</Table.Cell>
            <Table.Cell colSpan={4}>Larry the Bird</Table.Cell>
        </Table.Row>
    </Table.Body>
</Table>
```

## Props

### `Table`

```jsx
import {Table} from 'protrans-react-ui'
```

| Name | Type | Default | Description |
| ----------- | ----------- | ----------- | ----------- |
| className | string |  | Set a CSS class |
| hover | boolean | false | Allows hover effect on rows |
| striped | boolean | true | Enables alternating row colors |
| stickyColumns | boolean | false | Enables sticky columns |
| onMount | (React.Ref) => void |  | Allows scripts to fire when Table mounts. Also allows Table ref to be accessed. |

### `Table.Head`

| Name | Type | Default | Description |
| ----------- | ----------- | ----------- | ----------- |
| className | string |  | Set a CSS class |
| hide | boolean | false | Hide table head |
| onMount | (React.Ref) => void |  | Allows scripts to fire when Table mounts. Also allows Table ref to be accessed. |

### `Table.Column`

| Name | Type | Default | Description |
| ----------- | ----------- | ----------- | ----------- |
| width | string | 'auto' | Sets width of column |
| hide | boolean | false | Hide table head |
| onMount | (React.Ref) => void |  | Allows scripts to fire when Table mounts. Also allows Table ref to be accessed. |

### `Table.Body`

Table Body children are memoized.

### `Table.Row`

| Name | Type | Default | Description |
| ----------- | ----------- | ----------- | ----------- |
| data | object |  | description |
| forwardRef | React.MutableRefObject |  | description |
| className | string |  | description |
| isActive | boolean | false | description |
| isStripped | boolean | | description |
| selectable | boolean | false | description |
| noTextHighlight | boolean |  | description |
| onSelect | (data, isActive, e) => void |  | description |

### `Table.Cell`

| Name | Type | Default | Description |
| ----------- | ----------- | ----------- | ----------- |
| width | string | 'auto' | Sets width of column |
| hide | boolean | false | Hide table head |
| className | string |  | Set a CSS class |
| colSpan | number | 1 | Allows for cells to span multiple columns |
