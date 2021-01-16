<template>
    <Page>
        <ActionBar>
            <Label text="Test"/>
        </ActionBar>

        <ActivityIndicator :busy="!ready" />
    </Page>
</template>

<script>
export default {
    props: {
        text: {
            type: String
        }
    },
    data () {
        setTimeout(() => {
            this.$set(this, 'ready', true);
        }, 3000);
        return {
            ready: false
        };
    }
};
</script>