<template>
  <router-view/>
</template>

<style>
#app {
  font-family: "Inter", sans-serif;
  font-optical-sizing: auto;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  overflow-x: hidden;
}
h1{
  margin-bottom: 0px;
}
header{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.section-title{
    color: #4D4D4D;
    width: 45%;
    font-size: 1.5rem;
}
@media(max-width: 767.98px){
  .section-title{
    width: 85%;
  }
}
.description{
    color: #717171;
    font-size: .8rem;
}
a{
  cursor: pointer;
}
.medium{
    height: 37px;
    width: 97px;
    border-radius: 2px;
    background-color:#4CAF4F;
    font-size: .8rem;
    outline: none;
    border: none;
    color: white;
    cursor: pointer;
}
button{
  transition : 0.3s ease-in-out;
}
button:hover{
  transform: translateY(-5px);
}
</style>
