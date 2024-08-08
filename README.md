# portfolio
@import url('https://fonts.googleapis.com/css2?family=Akaya+Telivigala&family=Bebas+Neue&family=Noto+Sans&family=Permanent+Marker&family=Redressed&family=Roboto+Slab:wght@500&family=Roboto:wght@100&display=swap');



body {
  background: white;
  font-family: 'Noto Sans';
  font-size: 18px;
}

h1,
h2 {
  font-family: 'Roboto Slab';
  font-size: 1.5em;
  padding: 1em 0;
}

h2 {font-size:1.2em;}


nav{
  font-family: 'Roboto Slab';
  font-size:20px;
}

header {
  grid-area: heady;
  background-color:#D7D1FF;
}

header,
footer {
  text-align: center;
}

nav {
  grid-area: navvy;
  background-color:#FFF7DD;
}

header,
nav,
main,
aside,
footer {
  padding: 1.3em;
  border: 5px white solid;
}

main {
  max-height: 100%;
  grid-area: mainy;
  background-color: #EBC9E0;
}

footer {
  grid-area: footy;
  background-color: white;
}

nav ul {
  justify-content: space-around;
  display: flex;
  flex-flow: row nowrap;

}

nav ul li {
  list-style: none
}



*,
*:before,
*:after {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  background-color:white;
  display: grid;
  width: 100vw;
  height: 100vh;
  grid-template-columns:
   1fr       2fr       1fr;
  grid-template-areas:
  "heady     heady     heady"
  "navvy     navvy     navvy"
  "aside1    mainy     aside2"
  "aside1    mainy     aside2"
  "aside1    mainy     aside2"
  "footy     footy     footy";
}



#title{
  font-size:30px;
}

#aside1 {
  grid-area: aside1;
  background-color: #AAC0F5;
}
#aside2 {
  grid-area: aside2;
  background-color: #C9F0DD;
}


@media screen
  and (min-width: 641px)
  and (max-width: 900px)  {
.container {
grid-template-columns:
   1fr 1fr;
grid-template-areas:
  "heady heady"
  "navvy navvy"
  "mainy mainy"
  "aside1 aside2"
  "footy footy";
}


@media screen
  and (max-width: 640px)  {
.container {
grid-template-columns: 1fr;
grid-template-areas:
  "heady"
  "mainy"
  "aside1"
  "aside2"
  "navvy"
  "footy";
}
