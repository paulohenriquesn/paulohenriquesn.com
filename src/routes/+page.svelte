<script lang="ts">
  export const ssr = false;
</script>

<div class="container">
  <img src="eu.jpg" alt="me" id="img-me"/>
  <hgroup>
    <h1>Paulo Henrique <img src="/icons/duck.svg" alt="duck"/></h1>
    <h4 id="role">Desenvolvedor Backend</h4>
  </hgroup>
  <p class="tag">Estou disponivel para projetos e freelas</p>
  <nav>
    <ul>
      <li on:click={() => {
        window.open('http://linkedin.com/in/paulohenriquesn')
      }}><img src="/icons/linkedin.svg" alt="linkedin"></li>
      <li on:click={() => {
        window.open('http://github.com/paulohenriquesn')
      }}><img src="/icons/github.svg" alt="github"></li>
      <li on:click={() => {
        window.open('mailto:contact@paulohenriquesn.com')
      }}><img src="/icons/email.svg" alt="email"></li>
      <li on:click={() => {
        window.open('http://instagram.com/paulohs_n')
      }}><img src="/icons/instagram.svg" alt="instagram"></li>
    </ul>
  </nav>

  <article>
    <p class="tag red big">Algumas experiências</p>
    <p class="tag big left shadow"><img id="flag" src="/icons/spain.svg" alt="spain"/>  Blocks Revit - Tech Lead</p>
    <p class="tag big left shadow"><img id="flag" src="/icons/brazil.svg" alt="brazil"/>  Farmacias App By Grupo SC - Backend Engineer</p>
    <p class="tag big left shadow"><img id="flag" src="/icons/brazil.svg" alt="brazil"/>  Triad Systems - Full Stack Engineer</p>
    <p class="tag big left shadow"><img id="flag" src="/icons/brazil.svg" alt="brazil"/>  Athlete Training Center - Full Stack Engineer</p>
  </article>
</div>
<style>

  #img-me {
    width:200px;
    border-radius: 18px;
  }

.shadow {
  background-color: #2a2a2a;
}

.left{
  text-align: left !important;
  padding-left: 12px;
}

  #flag {
    width:12px;
  }

  article {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .big {
    width: 100%;
  }

  .small {
    width: 50%;
  }

  .red {
    background-color: #f2f2;
  }

  .tag {
    font-size: 9pt;
    border: 1px solid;
    text-align: center;
  }

  #role {
    opacity: 0.7;
  }

  * {
    font-family: monospace;
    color: white;
    font-size: 15pt;
  }

  hgroup h1 {
    display: flex;
    align-items: center;
    font-size: 22pt;
  }

  hgroup h1 img {
    width:32px;
    margin-left: 32px;
  }

  .container {
    margin: 10% auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  .container hgroup {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .container hgroup h4 {
    margin-top: -16px;
  }

  ul {
    display:flex;
    margin-left: -32px;
  }

  ul li {
    display: flex;
    align-items: center;
    padding: 10px 10px 10px;
    list-style: none;
  }

  ul li img {
    width:32px;
    padding-right: 12px;
    background-color: #fff;
    border-radius: 128px;
    padding-left: 12px;
    transition: all 500ms;
  }

  ul li img:hover {
    filter: brightness(0.7);
    cursor:pointer;
  }

  ul li a {
    opacity: 0.6;
    text-decoration: none;
    transition: all 500ms;
  }

  ul li a:hover {
    background-color: #000;
    padding:12px 12px 12px;
    opacity:100;
  }
  
  
  @media (max-width: 720px){
  #role {
    font-size: 12pt !important;
  }
}


</style>
