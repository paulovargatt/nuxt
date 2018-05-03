<template>

        <section class="post-list">
            <PostPreview :is-admin="IsAdmin" id="54" title="Vargatao" />
            <PostPreview />
            <PostPreview />
        </section>
</template>

<script>
    import PostPreview from '@/components/Posts/PostPreview'
    export default {
        components: {
            PostPreview
        },
        props: {
            isAdmin: {
                type: Boolean,
                default: false
            }
        }
    }
</script>


<style scoped>
    .post-list {
        display: flex;
        padding: 20px;
        box-sizing: border-box;
        flex-wrap: wrap;
        align-items: center;
        justify-content: center;
    }
</style>