<script>
    import { Button, Dropdown, DropdownItem, Chevron } from 'flowbite-svelte'
  </script>
  
  <Button><Chevron>Dropdown button</Chevron></Button>
  <Dropdown >
    <DropdownItem><a href="/code">code</a></DropdownItem>
    <DropdownItem>Settings</DropdownItem>
    <DropdownItem>Earnings</DropdownItem>
    <DropdownItem>Sign out</DropdownItem>
  </Dropdown>
<slot></slot>
