<template>
    <div id="Nav">
        <nav>
            <div class="check">
                <div class="title"><a href=""><img src="https://fontmeme.com/permalink/220405/325004c958092269dbfae5bbd18675f3.png" alt="netflix-font" border="0"></a></div>
                
                <div class="navigation">
                    <a>Accueil</a>
                    <a>Séries</a>
                    <a>Film</a>
                    <a>Nouveautés les plus regardées</a>
                    <a>Ma liste</a>
                </div>
            </div>

            <div class="research">
                <div><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-search" viewBox="0 0 16 16">
                <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"/>
                </svg></div>

                <div>DIRECT</div>

                <div>Jeunesse</div>

                <div><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-bell-fill" viewBox="0 0 16 16">
                <path d="M8 16a2 2 0 0 0 2-2H6a2 2 0 0 0 2 2zm.995-14.901a1 1 0 1 0-1.99 0A5.002 5.002 0 0 0 3 6c0 1.098-.5 6-2 7h14c-1.5-1-2-5.902-2-7 0-2.42-1.72-4.44-4.005-4.901z"/>
                </svg></div>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
  name: 'NavBar',
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Hubballi&family=Raleway:ital,wght@1,100&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Hubballi&family=Raleway:ital,wght@1,100&family=Roboto&display=swap');

#Nav {
    display: block;
    position: fixed;
    width: 100%;
    margin-top: -9vh;
}

#Nav nav{
    display: flex;
    flex-direction: row;
    background-color: #000;
    padding: 0.2vw;
    color: #fff;
}

.check {
    display: flex;
    justify-content: left;
    width: 50vw;
}

.title {
    font-family: 'Bebas Neue', cursive;
    margin-left: 2.5vw;
}

.navigation {
    font-family: 'Roboto', sans-serif;
    font-size: 0.9em;
    margin-top: 2vh;
}
.navigation a {
    margin-left: 1.8em;
}

.research {
    display: flex;
    justify-content: right;
    width: 50vw;
    margin-top: 2vh;
}
.research div {
    margin-right: 1.8em;
}
</style>