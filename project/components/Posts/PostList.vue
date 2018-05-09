<template>

        <section class="post-list">
            <PostPreview  id="54"
                          :is-admin="IsAdmin"
                          title="Vargatao"
                         previewText="PREVIEW TEXT" />
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
            },
            posts: {
                type: Array,
                required: true
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