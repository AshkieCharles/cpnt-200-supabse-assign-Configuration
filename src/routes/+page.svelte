<script>
  export let data;
  let { blog_post } = data;
</script>

{#each data.blog_post as blog_post}
  <h1>{blog_post.title} </h1>
  <h2> Posted by: {blog_post.author}</h2>
  <h3>Published on {blog_post.date_published}</h3>
  <div>
    <p>
      {blog_post.rich_text}
    </p>
    <h2>Summary</h2>
      <p>
        {blog_post.Summary}
      </p>
  </div>
  <div>
    <h2>
      Tags: 
    </h2>
    <p>
      {blog_post.blog_tags}
    </p>
  </div>
{/each}
