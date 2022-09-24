<template>
    <div>
        <button>
            <Link
                :href="route('homepage')"
                :class="{'font-bold': $page.component === 'Home'}"
            >
                Homepage
            </Link>
        </button>
        <button>
            <Link :href="route('about')"
                :class="{'font-bold': $page.component === 'About'}"
            >
                About
            </Link>
        </button>
        <button>
            <Link
                :href="route('contact')"
                :class="{'font-bold': $page.component === 'Contact'}"
            >
                Contact
            </Link>
        </button>

        <slot />
    </div>
</template>

<style>
    .font-bold { font-weight: bold }
</style>

<script>
export default {

}
</script>