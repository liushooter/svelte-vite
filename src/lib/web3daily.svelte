<script>
  import { onMount } from "svelte";
  // const endpoint = "https://jsonplaceholder.typicode.com/posts";
    const url = "http://db.rebase.network/web3daily/public/posts?_order=-id,-time&_page_size=50&_page=1"

    let posts = [];

    const opts =  {
      'Content-Type': 'application/json'
    }

    onMount(async function () {
      const response = await fetch(url, {headers: opts});
      console.log("response.status"  + response.status)
      const data = await response.json();
      console.log(data);
      posts = data;
    });

</script>


<div class="list-group list-group-checkable d-grid gap-2 border-0 w-auto">

  {#each posts as post}
  <div>
    <p></p>
  </div>
  <label class="list-group-item rounded-3 py-3">
    {post.title}
    <span class="small opacity-50">{post.time}</span>
    <span class="d-block small opacity-50">{post.url}</span>
    <p>{post.introduce}</p>
  </label>

  {/each}


</div>