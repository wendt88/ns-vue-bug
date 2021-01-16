<template>
    <Page>
        <ActionBar>
            <Label text="Home"/>
        </ActionBar>

        <GridLayout>
            <Button text="Go to Test" @tap="$navigateTo(Test, {
                props: {
                    text: 'Hi'
                }
            })" />
        </GridLayout>
    </Page>
</template>

<script>
    import Test from './Test';
    export default {
        data () {
            return {
                Test
            };
        }
    };
</script>
