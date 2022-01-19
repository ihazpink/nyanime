<script lang="ts">
  import Searchbar from "./_searchbar.svelte";
</script>

<style lang="scss">
  $topnavHeight: 3rem;

  nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: $topnavHeight;
            
    padding: 0.5rem;
    margin: 0;
             
    background-color: #181818;
    box-shadow: 0 0 20px black;
  }

  #icon {
    height: $topnavHeight;
    width: auto;
    flex: 1 1 0;
          
    img {
      height: $topnavHeight; 
      width: auto;
    }
  }

  #search {
    display: flex;
    justify-content: center;
    height: inherit;
    flex: 1 1 0;
  }

  #urls {
    flex: 1 1 0;
    text-align: right;
    
    a {
      color: whitesmoke;
      font-family: Arial, Helvetica, sans-serif;
      text-decoration: none;
      font-size: 1.25rem;
      padding: 0 10px;
    }
  }
</style>

<svelte:head>
  <title>Nyanime</title>
  <link rel="stylesheet" href="shared.css">
</svelte:head>

<nav>
  <a id="icon" href="/">
    <img src="favicon.png" alt="Favicon">
  </a>
  
  <div id="search">
    <Searchbar />
  </div>

  <div id="urls">
    <a href="about">About</a>
    <a href="upload">Upload</a>
    <a href="profile">My profile</a>
  </div>
</nav>

<slot></slot>