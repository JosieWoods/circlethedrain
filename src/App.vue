<template>
  <div class="bg-black">
  <div class="banner-1">
  <div class ="flex">
  <!--Logo and Social Buttons-->
  <div class="flex-col items-center justify-between w-5 mr-10">
        <div class="relative w-16 h-16 mr-5">
          <img
            class="rounded-full"
            src="./assets/ctdlogo.png"
          />
        <a href="https://www.instagram.com/circlethedrainband/">
          <img
            class="rounded-full size-10 ml-1 mt-1"
            src="./assets/instagram.png"
          />
          </a>
        <a href="https://open.spotify.com/artist/66rzOvJabQqzfYNO0xF0aK">
          <img
            class="w-12 h-8"
            src="./assets/spotify.png"
          />
          </a>
          </div>
      </div>
    <div><p class="text-white w-48"></p></div>
    <!-----End Logo----->
    <!-- NavBar -->
    <nav
      class="container px-6 mx-auto md:flex md:justify-between md:items-center"
    >
      <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
      <ul
        :class="showMenu ? 'flex' : 'flex object-top'"
        class="flex-col items-end space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0"
      >
        <li class="menu-button"><a href="#">Home</a></li>
        <li class="menu-button"><a href="#music" v-smooth-scroll>Music</a></li>
        <li class="menu-button">
          <a href="#video" v-smooth-scroll>Videos</a>
        </li>
        <li class="menu-button"><a href="#testimonials" v-smooth-scroll>Testimonials</a></li>
        <li class="menu-button"><a href="#about" v-smooth-scroll>About</a></li>
      </ul>
    </nav>
    <!-- End Navbar -->
    </div>
    </div>
    <div class="mainGif">
        <img
          class="size-2/3 mt-20"
          src="./assets/ctdslowgif.gif"
          alt="gif of Circle the Drain performing"
        />
      </div>

  <div class="banner-2 space-y-10 pb-20" id="music">
    <div>
    <h3 class="heading3 my-5 ml-2">Our Music</h3>
    <p class="text-left font-work_sans text-gray-600 font-semibold leading-relaxed ml-2">
    Stream these tunes!
      </p>
    </div>
    <div class="card">
      <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
        <h4 class="project-title item">Lil Stuart / Helium Tank</h4>
        <p class="font-work_sans pr-12">
          Enjoy our first release in the form of this double single!

          I found this mouse in my house, his name is Stuart, Lil' Stuart, and he got into the Helium
          supply! He's just sucked it all up! He's currently 20,000 feet in the air, if anyone has
          a helicopter please send it our way now!!!
        </p>
        <br>
        <a href="https://open.spotify.com/album/55XVE4ILyuIG2042BhU8eL?si=pPX4Qs5SRTeHhlBBVd06vg" class="text-sky-600 font-bold text-2xl tracking-wider mt-20">
          Listen Now!
        </a>
      </div>
      <div class="card-image bg-white-100">
        <img
          class="object-cover w-full h-full"
          src="./assets/mousef.png"
        />
      </div>
    </div>

    <div class="card">
      <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
        <h4 class="project-title item">Select Live Tracks</h4>
        <p class="font-work_sans pr-12">
          While we're workin' on our EP, enjoy some live tracks from some recent shows!! If you've been wanting to stream and scream about crabs, your time is now!!
        </p>
        <br>
        <a href="https://circlethedrainband.bandcamp.com/album/select-live-tracks-vol-1" class="text-sky-600 font-bold text-2xl tracking-wider">
          Check them out on Bandcamp!
        </a>
      </div>
      <div class="card-image">
        <img
          class="object-cover bg-white-100 w-full h-full"
          src="./assets/ctdlive.jpg"
        />
      </div>
    </div>
  </div>

  <div class="banner-2 ml-5" id="video">
    <div class="space-y-4 grid mt-5 mr-5">
      <h3 class="heading3 text-right">Videos</h3>
      <p class="text-right font-work_sans text-gray-600 font-semibold leading-relaxed">
        Check out some clips of us in action!
      </p>
    </div>

    <div class="max-w-6xl mx-auto px-8 py-16">
      <div class="flex justify-center">
      <div class="flex-col justify-center">
    <iframe width="360" height="185" src="https://www.youtube.com/embed/N8cMRRl258E?si=TtYr5BW6I4Vx9tMY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen class="mr-10"></iframe>
    <hr class="h-px my-8 mr-10 w-130 bg-white border-0 dark:bg-white">
    <iframe width="360" height="185" src="https://www.youtube.com/embed/PUdXtAge_84?si=iJd60jxk8OB26dqy" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>
    </div>
      <div class="relative">
      </div>
    </div>
  </div>

  <div class="banner-2" id="testimonials">
    <div class="space-y-4 grid mt-5">
      <h3 class="heading3 text-left ml-1">Testimonials</h3>
      <p class="text-left font-work_sans text-gray-600 font-semibold leading-relaxed ml-1">
        Kind words from amazing people 🥹
      </p>
    </div>
    <div class="max-w-6xl mx-auto px-8 py-16">
      <div class="relative">
        <div class="relative lg:flex rounded-lg overflow-hidden">
        <a href="http://www.theauricular.com/news/rva-shows-you-must-see-this-week-march-27-april-2/" class="size-4/5 mr-10">
        <img
          src="./assets/ctdtestone.png"
        />
        </a>
          <div
            class="h-56 lg:h-auto relative flex items-center justify-center size=2/5"
          ></div>
          <a href="https://www.instagram.com/circlethedrainband/">
          <img
          src="./assets/ctdTestTwo.png"
        />
        </a>
        </div>
      </div>
    </div>
  </div>

<div class="banner-2 space-y-10 pb-5" id="music">
<h3 class="heading3 text-right mr-5">About Us</h3>
</div>
<div class="flex-col ml-5">
<div class="flex justify-center">
    <img
      class="size-2/5 ml-5"
      src="./assets/ctdtree.png"
    />
  <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
      <p class="font-work_sans text-white">
        Hey y'all, we're Circle the Drain! We're a genre hoppin' rock band from Richmond, VA singin' about a lil' mouse, crabs, honey and more!
        <br>
        <br />
        Based in rock with a focus on emo, indie, funk, and metal! (but not at the same time!)
        <br>
        <br />
        Venues Played: The Camel, The Canal Club, Cobra Cabana, Bandito's
        <br>
        <br />
        Bands We've Performed With: Ekko Astral, Flight Club, Crush Fund, Ten Pound Snail, Dogs on Shady Lane, Los Malcriados, Boy Scout Marie, Hemmingway Lane, Tiny the Dream
      </p>
    </div>
  </div>
  </div>

  <div class="banner-1 flex h-full items-center">
    <div class="w-7/12">
    <div class="flex">
      <h2 class="text-orange-200 md:text-6xl text-2xl font-Eczar mb-5 font-bold">
        Crabs, crabs, crabs, please!
        In my mouth yeah;
        I'm allergic to shellfish, I wanna die!
        Just like Amelia Earhart, take me crabs!
      </h2>
      </div>
      <div class="pb-5">
      <p class="text-white">For booking inquiries: </p>
      <a class="underline text-small text-sky-200 font-work_sans"
        >circlethedrainband@gmail.com</a
      >
      </div>
    </div>
    <div class="size-2/5">
      <div class="flex flex-wrap justify-end gap-2">
      <img
            class="pb-20 pl-5"
            src="./assets/ctdposter.png"
          />
      </div>
    </div>
  </div>
</div>
</template>
<script>

  export default {
    data() {
      return {
        showMenu: false,
      }
    },
  }
</script>
