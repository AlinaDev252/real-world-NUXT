<template>
  <div class="nav">
    <nuxt-link to="/" class="brand">Real World Events</nuxt-link>
    <nav>
      <nuxt-link to="/">List</nuxt-link> |
      <nuxt-link to="/event/create">Create</nuxt-link> |
      <nuxt-link to="/">
        <img
          class="pic"
          src="https://avataaars.io/?avatarStyle=Circle&topType=LongHairCurvy&accessoriesType=Blank&hairColor=BrownDark&facialHairType=Blank&clotheType=Hoodie&clotheColor=PastelRed&eyeType=Side&eyebrowType=RaisedExcitedNatural&mouthType=Default&skinColor=Light"
        />
      </nuxt-link>
    </nav>
  </div>
</template>

<style scoped>
.brand {
  font-family: "Montserrat", sans-serif;
  font-weight: 700;
  font-size: 1.5em;
  color: #39b982;
  text-decoration: none;
}
.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 60px;
}
.nav .nav-item {
  box-sizing: border-box;
  margin: 0 5px;
  color: rgba(0, 0, 0, 0.5);
  text-decoration: none;
}
.nav .nav-item.router-link-exact-active {
  color: #39b982;
  border-bottom: solid 2px #39b982;
}
.nav a {
  display: inline-block;
}
.nav .pic {
  width: 2em;
  height: 1.8em;
  margin-bottom: -1vh;
}
</style>
