<template>
  <div class="container">
    <div class="pv3">
      <nav
        class="
          flex flex-wrap
          justify-between
          items-center
          w-80
          mv0
          ml-auto
          mr-auto
          justify-center-m
          flex-auto-m
          content-start-l
          flex-nowrap-l
          menu
          relative
          static-l
        "
      >
        <a href="#" class="flex items-center logo order-0-l">
          <img
            src="../static/images/logo.svg"
            class="db mw-100 h-auto"
            alt=""
          />
        </a>

        <ul
          id="listing"
          class="
            list
            p10
            order-3
            dn
            tc
            w-100
            top-2 top-0-l
            static-l
            flex-l
            w-auto-l
            flex-row-l
            order-1-l
            item
            mt3
            mt0-l
          "
        >
          <li class="pointer mr3-l dib-l"><a href="#" class="db"></a>Home</li>
          <li class="pointer mr3-l dib-l">
            <a href="#" class="db"></a>Contact
          </li>
          <li class="pointer mr3-l dib-l"><a href="#" class="db"></a>About</li>
          <li class="pointer mr3-l dib-l"><a href="#" class="db"></a>Blog</li>
          <li class="pointer dib-l"><a href="#" class="db"></a>Careers</li>
        </ul>

        <button
          class="
            nav-btn
            white
            pv2
            ph3
            bn
            br-pill
            pointer
            dn
            db-l
            order-3 order-1-l
            relative-l
            w-auto-l
          "
        >
          Request Invite
        </button>

        <div
          class="toggle order-1 db dn-l flex-auto-m tr-m order-2-m"
          @click="togo()"
        >
          <a href="#"><i class="fas fa-bars"></i></a>
        </div>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    togo() {
      const toggle = document.querySelector('.toggle')
      const menu = document.querySelector('.menu')
      function toggleMenu() {
        if (menu.classList.contains('active')) {
          menu.classList.remove('active')
          toggle.querySelector('a').innerHTML = "<i class='fas fa-bars'></i>"
          console.log('clicked')
        } else {
          menu.classList.add('active')
          toggle.querySelector('a').innerHTML = "<i class='fas fa-times'></i>"
          console.log('not clicked')
        }
      }
      toggleMenu()
    },
  },
  mounted() {
    this.togo()
  },
}
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

.active .item {
  display: block;
}
</style>
