<div class="one">
  <div class="top" />
  <div class="mid"><a href="/">€</a></div>
  <div class="bot" />
</div>

<style>
  a, a:visited {
    color: hsl(268, 87%, 3%);
  }
  a:hover {
    font-size: 1.6rem;
    padding: 0.2em;
  }
  .one {
    font-size: 1rem;
    display: flex;
    flex-direction: row;
    width: 3rem;
    height: 3rem;
    background-color: hsl(204, 79%, 74%);
    border-radius: 25%;
    z-index: 4;
  }
  .top {
    border-radius: 25%;
    align-self: flex-start;
    width: 1rem;
    height: 1rem;
    background-color: hsl(258, 71%, 38%);
  }
  .mid {
    padding: 0.5em;
    align-self: center;
    width: fit-content;
    background-color: hsl(76, 71%, 38%);
    border-radius: 50%;
  }
  .bot {
    border-radius: 25%;
    align-self: flex-end;
    width: 1rem;
    height: 1rem;
    background-color: hsl(0, 71%, 38%);
  }
</style>
