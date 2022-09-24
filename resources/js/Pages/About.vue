<template>
    <Head>
        <title>{{ title }} - My awesome app</title>
    </Head>

    <AppLayout>
        <h1>This is: {{ title }}</h1>
    </AppLayout>
</template>

<script>
import AppLayout from '../Layouts/AppLayout.vue';

export default {
    components: { AppLayout },

    props: {
        title: String,
    },
}
</script>