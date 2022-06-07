<script>
import CssProvider from "./CSSProvider.svelte";
import DropdownMenu from "./DropdownMenu.svelte";

import Navbar from "./Navbar.svelte";
import NavItem from "./NavItem.svelte";


</script>

<CssProvider>
    <Navbar>
        <NavItem icon="🤣" />
        <NavItem icon="🤣" />   
        <NavItem icon="🤣" />
        <NavItem icon="🤣">   
            <DropdownMenu />
        </NavItem>
    </Navbar>
</CssProvider>