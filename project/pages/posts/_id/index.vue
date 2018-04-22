<template>
    <section class="single-post-page">
        <div class="post">
            <h1 class="title-post">Oi</h1>
        </div>
        <article class="post-details">
            <div class="post-detail">
                <span>Criação</span>
            </div>
            <div class="post-detail">
                <span>Criação</span>
            </div>
        </article>

        <div class="post-content">
            <div>Lorem ipsum dolor sit amet, consectetur adipisicing elit. A dolorum ducimus sequi vero vitae! Aperiam
                delectus eaque itaque laborum magni, molestiae, natus necessitatibus nulla obcaecati omnis quae quasi,
                ullam ut!
            </div>
            <div>Accusantium aliquid corporis dolores doloribus non nulla quod. A accusantium ad animi architecto
                blanditiis, eligendi et eum illo in quos rem, temporibus totam voluptas. Ab aliquam hic odio quam
                voluptates!
            </div>
            <div>Ad animi, consectetur deserunt doloremque et ex facere impedit, ipsa, nam officiis possimus quibusdam
                temporibus ullam ut vel vero voluptas! Corporis enim error illo, maxime nihil optio recusandae repellat
                tempore.
            </div>
        </div>

            <section class="post-feedback">
                <p><span>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus aspernatur dicta dolor eaque eius excepturi, iure magni molestias natus odio officia pariatur perferendis quas quasi quia sit, tempore, vel voluptates!</span><span>Aspernatur dolores error modi neque nisi voluptatem. Accusamus adipisci aliquid aperiam assumenda at autem, cumque doloremque, esse in magnam nam quam quod quos sit sunt voluptas voluptate. Culpa, sapiente, sit?</span><span>Distinctio doloribus illum in maxime modi mollitia nam obcaecati perferendis quis quo sed sunt ullam, voluptates! Ab aut consectetur dolores, facilis harum iste nostrum placeat quam qui quos veniam, vero.</span><span>Aliquid amet cupiditate facere, labore modi quidem repellendus! Ab aliquam amet architecto asperiores cum delectus esse, exercitationem facilis fugiat harum illum magni placeat quas quidem repellendus. Natus soluta unde vel?</span><span>Corporis deleniti, dolor ex expedita impedit ipsam perferendis perspiciatis placeat quis ratione recusandae rerum temporibus tenetur. Alias aliquam aut cupiditate explicabo, fugit illum incidunt nobis obcaecati, quas quidem veritatis voluptatum?</span><span>Assumenda autem beatae blanditiis commodi consectetur consequatur corporis ducimus, et, exercitationem laudantium maxime mollitia nam odio officiis omnis pariatur quaerat recusandae, repellat repudiandae suscipit tenetur voluptas voluptates! Maxime, officia praesentium!</span><span>Adipisci asperiores beatae eum eveniet fugit harum ipsa iusto laboriosam laudantium magni quibusdam similique, suscipit unde vero voluptatum. Aliquid aperiam ea esse illum inventore nesciunt odio, officia optio tenetur voluptatem?</span></p>
            </section>
    </section>
</template>

<style scoped>

    .single-post-page {
        padding: 30px;
        text-align: center;
        box-sizing: border-box;
    }

    .post {
        width: 100%;
    }

    @media (min-width: 768px) {
        .post {
            width: 600px;
            margin: auto;
        }
    }

    .post-title {
        margin: 0;
    }

    .post-details {
        padding: 10px;
        box-sizing: border-box;
        border-bottom: 3px solid #ccc;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }

    @media (min-width: 768px) {
        .post-details {
            flex-direction: row;
        }
    }

    .post-detail {
        color: rgb(88, 88, 88);
        margin: 0 10px;
    }

    .post-feedback a {
        color: red;
        text-decoration: none;
    }

    .post-feedback a:hover,
    .post-feedback a:active {
        color: salmon;
    }

</style>