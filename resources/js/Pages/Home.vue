<template>
    <Head>
        <title>{{ title }} - My awesome app</title>
    </Head>

    <div>
        <div>
            <button>
                <Link :href="route('homepage')">Homepage</Link>
            </button>
            <button>
                <Link :href="route('about')">About</Link>
            </button>
            <button>
                <Link :href="route('contact')">Contact</Link>
            </button>
        </div>

        <h1>This is: {{ title }}</h1>
    </div>
</template>

<script>
export default {
    props: {
        title: String,
    }
}
</script>