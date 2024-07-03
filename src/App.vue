<template>
  <div class="bg-black">
  <div class="banner-1">
    <!-- NavBar -->
    <nav
      class="container px-6 mx-auto md:flex md:justify-between md:items-center"
    >
      <div class="flex-col items-center justify-between">
        <div class="relative w-16 h-16">
          <img
            class="rounded-full"
            src="./assets/CtD Logo.png"
            alt="user image"
          />
        <a href="https://www.instagram.com/circlethedrainband/">
          <img
            class="rounded-full size-10 ml-1 mt-1"
            src="./assets/instagram.png"
            alt="user image"
          />
          </a>
        <a href="https://open.spotify.com/artist/66rzOvJabQqzfYNO0xF0aK">
          <img
            class="w-12 h-8"
            src="./assets/spotify.png"
            alt="user image"
          />
          </a>
          </div>
        <!-- Mobile menu button -->
        <div @click="showMenu = !showMenu" class="flex md:hidden">
          <button
            type="button"
            class="text-white-800 hover:text-white-400 focus:outline-none focus:text-white-400"
          >
            <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
              <path
                fill-rule="evenodd"
                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
              ></path>
            </svg>
          </button>
        </div>
      </div>
      <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
      <ul
        :class="showMenu ? 'flex' : 'hidden'"
        class="flex-col items-end mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0"
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
    <div class="mainGif">
        <img
          class="size-2/3"
          src="./assets/CtD Slow Gif.gif"
          alt="gif of Circle the Drain performing"
        />
      </div>

  <div class="banner-2 space-y-10 pb-20" id="music">
    <div>
    <h3 class="heading3 my-5">Our Music</h3>
    <p class="text-left font-work_sans text-gray-600 font-semibold leading-relaxed">
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
          class="object-cover w-full h-48 md:h-96"
          src="./assets/CtD Live.jpg"
        />
      </div>
    </div>
  </div>

  <div class="banner-2" id="video">
    <div class="space-y-4 grid mt-5">
      <h3 class="heading3 text-right">Videos</h3>
      <p class="text-right font-work_sans text-gray-600 font-semibold leading-relaxed">
        Check out some clips of us in action!
      </p>
    </div>

    <div class="max-w-6xl mx-auto px-8 py-16">
      <div>
      <div class="flex">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/N8cMRRl258E?si=TtYr5BW6I4Vx9tMY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen class="mr-10"></iframe>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/PUdXtAge_84?si=iJd60jxk8OB26dqy" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>
    </div>
      <div class="relative">
      </div>
    </div>
  </div>

  <div class="banner-2" id="testimonials">
    <div class="space-y-4 grid mt-5">
      <h3 class="heading3 text-left">Testimonials</h3>
      <p class="text-left font-work_sans text-gray-600 font-semibold leading-relaxed">
        Kind words from amazing people 🥹
      </p>
    </div>
    <div class="max-w-6xl mx-auto px-8 py-16">
      <div class="relative">
        <div class="relative lg:flex rounded-lg overflow-hidden">
        <a href="http://www.theauricular.com/news/rva-shows-you-must-see-this-week-march-27-april-2/" class="size-4/5 mr-10">
        <img
          src="./assets/CtD Testimonial 1.PNG"
          alt="gif of Circle the Drain performing"
        />
        </a>
          <div
            class="h-56 lg:h-auto relative flex items-center justify-center size=2/5"
          ></div>
          <a href="https://www.instagram.com/circlethedrainband/">
          <img
          src="./assets/CtD Testimonial 2.PNG"
          alt="gif of Circle the Drain performing"
        />
        </a>
        </div>
      </div>
    </div>
  </div>

  <div class="banner-2 md:flex items-center md:justify-evenly" id="about">
    <img
      class="md:h-[500px] h-[400px]"
      src="./assets/CtD Tree.jpeg"
      alt="user image"
    />
    <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
      <h4 class="project-title item">About Us</h4>
      <p class="font-work_sans">
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

  <div class="banner-1 flex h-full items-center">
    <div class="w-7/12 p-12">
    <div class="flex">
      <h2 class="text-orange-200 md:text-6xl text-2xl font-Eczar mb-5 font-bold">
        Crabs, crabs, crabs, please!
        In my mouth yeah;
        I'm allergic to shellfish, I wanna die!
        Just like Amelia Earhart, take me crabs!
      </h2>
      </div>
      <p class="text-white">For booking inquiries: </p>
      <a class="underline text-2xl text-sky-200 font-work_sans"
        >circlethedrainband@gmail.com</a
      >
    </div>
    <div class="w-5/12 pr-28">
      <div class="flex flex-wrap justify-end gap-2">
      <img
            class=""
            src="./assets/CtD Poster.png"
            alt="user image"
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
