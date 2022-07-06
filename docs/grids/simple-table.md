---
sidebar_position: 1
---

# Simple Table

Create simple Tables with columns and rows in PTRUI.

### Table

Main container comp for Tables.

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
