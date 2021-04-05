<script lang="ts">
    import { HeaderNav, HeaderNavItem, HeaderNavMenu, Content, Grid, Row, Column, Header, SkipToContent} from "carbon-components-svelte";
    import {UserAvatarFilled32} from "carbon-icons-svelte";
</script>

<Header company="Bulletin">
    <div slot="skip-to-content">
        <SkipToContent />
    </div>

    <HeaderNav>
        <HeaderNavMenu text="Menu">
            <HeaderNavItem href="/" text="home" />
            <HeaderNavItem href="/" text="account" />
            <HeaderNavItem href="/" text="settings" />
        </HeaderNavMenu>
    </HeaderNav>
    <Grid container justify="flex-end">
        <UserAvatarFilled32 justify="flex-end"/>
    </Grid>

</Header>

<Content>
    <Grid>
        <Row>
            <Column>
                <h1>Welcome</h1>
            </Column>
        </Row>
    </Grid>
</Content>
