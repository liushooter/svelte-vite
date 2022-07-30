<script>
  import svelteLogo from './assets/svelte.svg'
  import Counter from './lib/Counter.svelte'
  import Daily from './lib/web3daily.svelte'
</script>

<div class="container">

  <header class="d-flex flex-wrap align-items-center justify-content-center justify-content-md-between py-3 mb-4 border-bottom">
    <a href="/" class="d-flex align-items-center col-md-3 mb-2 mb-md-0 text-dark text-decoration-none">
      <img src=""/>
    </a>

    <ul class="nav col-12 col-md-auto mb-2 justify-content-center mb-md-0">
      <li><a href="/" class="nav-link px-2 link-secondary">Home</a></li>
      <li><a href="./web3daily.html" class="nav-link px-2 link-dark">Web3Daily</a></li>
      <li><a href="./jobs.html" class="nav-link px-2 link-dark">Jobs</a></li>
      <li><a href="#" class="nav-link px-2 link-dark">Events</a></li>
      <li><a href="#" class="nav-link px-2 link-dark">Videos</a></li>
    </ul>

    <div class="col-md-3 text-end">
      <button type="button" class="btn btn-outline-primary me-2">Login</button>
      <button type="button" class="btn btn-primary">Sign-up</button>
    </div>
  </header>
  <!--  -->
  <h1>Hello, Bootstrap and Webpack!</h1>
  <button class="btn btn-primary">Primary button</button>

  <div class="text-center">
    <div class="row">
      <div class="col-8">
        <Daily/>
      </div>
      <div class="col-4">col-4</div>
    </div>
  </div>
</div>

<style>
 
</style>
