<template>
  <div class="container">
    <div class="pv3">
      <nav class="flex justify-between w-80 mv0 ml-auto mr-auto">
        <a href="#" class="flex items-center">
          <img
            src="../static/images/logo.svg"
            class="db mw-100 h-auto"
            alt=""
          />
        </a>

        <ul class="list p10 flex-grow flex items-center">
          <li class="dib pointer mr4"><a href="#"></a>Home</li>
          <li class="dib pointer mr4"><a href="#"></a>About</li>
          <li class="dib pointer mr4"><a href="#"></a>Contact</li>
          <li class="dib pointer mr4"><a href="#"></a>Blog</li>
          <li class="dib pointer"><a href="#"></a>Careers</li>
        </ul>

        <button
          class="nav-btn flex items-center white pv2 ph3 bn br-pill pointer"
        >
          Request Invite
        </button>
      </nav>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
nav ul li {
  color: hsl(233, 8%, 62%);
}

nav ul li:hover {
  color: hsl(233, 26%, 24%);
}

nav button {
  font-weight: 700;
  background: rgb(49, 211, 92);
  background: linear-gradient(
    90deg,
    rgba(49, 211, 92, 1) 35%,
    rgba(43, 183, 218, 1) 100%
  );
}
</style>
