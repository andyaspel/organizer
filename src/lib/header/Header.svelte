<script>
    import Logo from "./Logo.svelte";
  </script>
  
  <header class="header">
    <div class="logo"><Logo /></div>
    <h1 class="page-title">page title</h1>
    <nav class="nav-bar">
      <a href="/">link button</a>
      <a href="/about">link button</a>
      <a href="/contacts">link button</a>
    </nav>
  </header>
  
  <style>
    .header {
      display: grid;
      grid-gap: 0.1em;
      grid-template-columns: repeat(6 ,1fr);
      grid-template-areas: 'logo title title title title nav ';
      align-content: space-between;
      box-sizing: inherit;
      font-size: 1rem;
      color: hsl(60, 16%, 87%);
      background-color: hsl(240, 91%, 17%);
      border: 1px solid hsl(256, 62%, 58%);
      max-height: 16vh;
     
    }
    .page-title {
      justify-self: center;
      margin:1rem ;
      grid-area: title;
      font-size: 3.2em;
      letter-spacing: 0.1em;
    }
    .logo {
      grid-area: logo;
      align-self: center;
      padding-left:  1em;
      margin:1rem;
      max-width: 64px;

    }
    .nav-bar {
      grid-area: nav;
      display: flex;
      flex-direction: column;
      margin: 1rem ;
      align-self: center;
      border: 0.2rem solid hsl(226, 63%, 84%);
    }
    a {
      color: hsl(60, 16%, 87%);
      padding-bottom: 0.3em;
    }
    a:hover {
      color: hsl(90, 42%, 48%);
      text-decoration: none;
    }
    a:visited {
      color: hsl(258, 19%, 89%);
      border: 0.2rem solid hsl(192, 82%, 32%);
    }
  </style>
  