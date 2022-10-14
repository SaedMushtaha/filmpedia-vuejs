<template>
  <div>
    <nav
      class="navbar navbar-expand-lg shadow-md py-2 top-0 inset-x-0 z-50 h-20 text-white bg-blue-600 font-medium flex items-center w-full justify-between"
    >
      <div class="px-6 w-full flex flex-wrap items-center justify-between">
        <div class="flex items-center">
          <button
            class="navbar-toggler border-0 py-3 lg:hidden leading-none text-xl bg-transparent text-white transition-shadow duration-150 ease-in-out mr-2"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarSupportedContentY"
            aria-controls="navbarSupportedContentY"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <svg
              aria-hidden="true"
              focusable="false"
              data-prefix="fas"
              class="w-5"
              role="img"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 448 512"
            >
              <path
                fill="currentColor"
                d="M16 132h416c8.837 0 16-7.163 16-16V76c0-8.837-7.163-16-16-16H16C7.163 60 0 67.163 0 76v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16z"
              ></path>
            </svg>
          </button>
        </div>
        <div
          class="navbar-collapse collapse grow items-center"
          id="navbarSupportedContentY"
        >
          <ul class="navbar-nav mr-auto lg:flex lg:flex-row">
            <li class="nav-item">
              <a
                class="nav-link block pr-2 lg:px-2 py-2 text-white transition duration-150 ease-in-out"
                href="#!"
                data-mdb-ripple="true"
                data-mdb-ripple-color="light"
                >Login &nbsp;
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  strokeWidth="{1.5}"
                  stroke="currentColor"
                  className="w-6 h-6"
                >
                  <path
                    strokeLinecap="round"
                    strokeLinejoin="round"
                    d="M17.982 18.725A7.488 7.488 0 0012 15.75a7.488 7.488 0 00-5.982 2.975m11.963 0a9 9 0 10-11.963 0m11.963 0A8.966 8.966 0 0112 21a8.966 8.966 0 01-5.982-2.275M15 9.75a3 3 0 11-6 0 3 3 0 016 0z"
                  />
                </svg>
              </a>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <aside
      class="w-64 text-black bg-white-700 fixed inset-y-0 overflow-x-hidden overflow-y-auto sm:block"
      id="style-11"
    >
      <div class="w-full h-full shadow-md bg-white px-1 absolute ">
        <div class="divide-y divide-gray-400 hover:divide-y-8 ">
          <div class="flex items-center mx-8 mt-6">
            <a
              href="#"
              class="flex items-center pl-2.5 mb-5 justify-self-center"
            >
              <img
                src="https://filmpedia.saedmu.com/static/media/FilmPedia.65883d147f76614fba5e.png"
                class="h-16 w-22 self-center"
                alt="Film pediaLogo"
              />
            </a>
          </div>
          <ul
            class="relative space-y-2 border-t border-gray-200 dark:border-gray-700"
          >
            <p class="font-sans font-bold text-left ml-2 text-gray-600">
              Category
            </p>
            <div v-for="list of sideitems" :key="list.label">
              <li class="relative">
                <a
                  class="flex items-center text-sm py-4 px-6 h-12 overflow-hidden text-gray-700 text-ellipsis whitespace-nowrap rounded hover:text-gray-900 hover:bg-gray-100 transition duration-300 ease-in-out"
                  href="#!"
                  data-mdb-ripple="true"
                  data-mdb-ripple-color="dark"
                >
                  <img class="w-8 h-8 mr-6" :src="list.src" />
                  <span class="text-base font-medium">{{ list.label }}</span>
                </a>
              </li>
            </div>
          </ul>
          <ul
            class="relative space-y-2 border-t border-gray-200 dark:border-gray-700"
          >
            <p class="font-sans font-bold text-left ml-2 text-gray-600">
              Genres
            </p>
            <div v-for="list of sidegenres" :key="list.label">
              <li class="relative">
                <a
                  class="flex items-center text-sm py-4 px-6 h-12 overflow-hidden text-gray-700 text-ellipsis whitespace-nowrap rounded hover:text-gray-900 hover:bg-gray-100 transition duration-300 ease-in-out"
                  href="#!"
                  data-mdb-ripple="true"
                  data-mdb-ripple-color="dark"
                >
                  <img class="w-8 h-8 mr-6" :src="list.src" />
                  <span class="text-base font-medium">{{ list.label }}</span>
                </a>
              </li>
            </div>
          </ul>

          <ul
            class="relative space-y-2 border-t border-gray-200 dark:border-gray-700"
          ></ul>
        </div>
      </div>
    </aside>

    <main class="sm:pl-64">
      <div class="p-4 flex justify-center">
        <div
          class=" bg-white w-96 rounded shadow font-semibold text-center hover:shadow-md"
        >
          <a href="#">
            <div class="relative">
              <img
                class=" max-w-3xl rounded-lg shadow-xl dark:shadow-gray-800 mx-auto"
                style="filter: brightness(0.6);"
                src="https://image.tmdb.org/t/p/original//5hoS3nEkGGXUfmnu39yw1k52JX5.jpg"
              />
              <figcaption
                style="margin-left: 150px"
                class="absolute max-w-md bottom-0 z-90 bg-black/50 px-5 py-2 text-white"
              >
                <h1 class="text-xl font-bold">
                  Fullmetal Alchemist: The Final Alchemy
                </h1>
                <p class="mt-1 italic text-sm font-light">
                  The Elric brothers’ long and winding journey comes to a close
                  in this epic finale, where they must face off against an
                  unworldly, nationwide threat.
                </p>
              </figcaption>
            </div>
          </a>

          <div class="flex flex-wrap justify-around">
            <div v-for="img of imgs" :key="img.title" class="w-48 bg-white ">
              <img
                :src="img.poster"
                class="my-8 rounded-md transform hover: transition duration-200 hover:scale-110"
                alt=""
              />
              <h3 class="text-xl font-extrabold">{{ img.title }}</h3>
              <div class="flex mb-5 mx-8">
                <svg
                  aria-hidden="true"
                  class="w-5 h-5 text-yellow-400"
                  fill="currentColor"
                  viewBox="0 0 20 20"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <title>First star</title>
                  <path
                    d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"
                  ></path>
                </svg>
                <svg
                  aria-hidden="true"
                  class="w-5 h-5 text-yellow-400"
                  fill="currentColor"
                  viewBox="0 0 20 20"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <title>Second star</title>
                  <path
                    d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"
                  ></path>
                </svg>
                <svg
                  aria-hidden="true"
                  class="w-5 h-5 text-yellow-400"
                  fill="currentColor"
                  viewBox="0 0 20 20"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <title>Third star</title>
                  <path
                    d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"
                  ></path>
                </svg>
                <svg
                  aria-hidden="true"
                  class="w-5 h-5 text-yellow-400"
                  fill="currentColor"
                  viewBox="0 0 20 20"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <title>Fourth star</title>
                  <path
                    d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"
                  ></path>
                </svg>
                <svg
                  aria-hidden="true"
                  class="w-5 h-5 text-gray-300 dark:text-gray-500"
                  fill="currentColor"
                  viewBox="0 0 20 20"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <title>Fifth star</title>
                  <path
                    d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"
                  ></path>
                </svg>
              </div>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<style>
#style-11::-webkit-scrollbar-track {
  -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
  background-color: #f5f5f5;
  border-radius: 10px;
}

#style-11::-webkit-scrollbar {
  width: 10px;
  background-color: #f5f5f5;
}

#style-11::-webkit-scrollbar-thumb {
  background-color: #3182ce;
  border-radius: 10px;
  background-image: -webkit-linear-gradient(
    0deg,
    rgba(255, 255, 255, 0.5) 25%,
    transparent 25%,
    transparent 50%,
    rgba(255, 255, 255, 0.5) 50%,
    rgba(255, 255, 255, 0.5) 75%,
    transparent 75%,
    transparent
  );
}

.image :hover {
  transform: scale(1.05);
}

figure {
  width: 300px;
  height: 200px;
  margin: 0;
  padding: 0;
  background: #fff;
  overflow: hidden;
}
figure:hover + span {
  bottom: -36px;
  opacity: 1;
  transform: scale(1.05);
}

.column {
  margin: 15px 15px 0;
  padding: 0;
}
.column:last-child {
  padding-bottom: 60px;
}
.column::after {
  content: "";
  clear: both;
  display: block;
}
.column div {
  position: relative;
  float: left;
  width: 300px;
  height: 200px;
  margin: 0 0 0 25px;
  padding: 0;
}
.column div:first-child {
  margin-left: 0;
}
.column div span {
  position: absolute;
  bottom: -20px;
  left: 0;
  z-index: -1;
  display: block;
  width: 300px;
  margin: 0;
  padding: 0;
  color: #444;
  font-size: 18px;
  text-decoration: none;
  text-align: center;
  -webkit-transition: 0.3s ease-in-out;
  transition: 0.3s ease-in-out;
  opacity: 0;
}

/* Shine */
.hover14 figure {
  position: relative;
}
.hover14 figure::before {
  position: absolute;
  top: 0;
  left: -75%;
  z-index: 2;
  display: block;
  content: "";
  width: 50%;
  height: 100%;
  background: -webkit-linear-gradient(
    left,
    rgba(255, 255, 255, 0) 0%,
    rgba(255, 255, 255, 0.3) 100%
  );
  background: linear-gradient(
    to right,
    rgba(255, 255, 255, 0) 0%,
    rgba(255, 255, 255, 0.3) 100%
  );
  -webkit-transform: skewX(-25deg);
  transform: skewX(-25deg);
}
.hover14 figure:hover::before {
  -webkit-animation: shine 0.75s;
  animation: shine 0.75s;
  transform: scale(1.05);
}
@-webkit-keyframes shine {
  100% {
    left: 125%;
  }
}
@keyframes shine {
  100% {
    left: 125%;
  }
}
</style>

<script>
const popURL =
  "https://api.themoviedb.org/3/discover/movie?sort_by=popularity.desc&api_key=04c35731a5ee918f014970082a0088b1&page=1";
const bg = "https://image.tmdb.org/t/p/w1280";
const searchURL =
  "https://api.themoviedb.org/3/search/movie?&api_key=04c35731a5ee918f014970082a0088b1&query=";
const imgTest =
  "https://image.tmdb.org/t/p/w1280/ugZW8ocsrfgI95pnQ7wrmKDxIe.jpg";
export default {
  data: () => ({
    imgTest: imgTest,
    imgs: [],
    searchTerm: "",
    sideitems: [
      {
        label: "Popular",
        src:
          "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAABmJLR0QA/wD/AP+gvaeTAAABLUlEQVR4nO3bwU7CQBhGUTS+/yvrWhfaMjK5/XvOGhLgpilfmnk8AAAA9no78JrPl3+Ke/n1N3/f9Sk4RpAYQWI+nnjPX/edn/ecI/epKzn7/U7dg10hMYLECBIjSIwgMc/8y7Lcv/vX38MVEiNIjCAxO5b6dJb6ZILECBIjSIwgMZb6Okt9MkFiBImx1NdZ6pMJEiNIjCAxgsRY6uss9ckEiREkxlJfZ6lPJkiMIDGCxAgS45z6fs6pX4kgMYLEOKd+nnPqdyJIjCAxgsQIEuOZ+jrP1CcTJEaQGM/U11nqkwkSI0iMIDGCxFjq6yz1yQSJESTGUl9nqU8mSIwgMYLECBJjqa+z1CcTJEaQGEt9naU+mSAxgsQIEiNIjHPq+zmnfiWCxAgCAABwc18uQSG2e/tM0QAAAABJRU5ErkJggg==",
      },
      {
        label: "Top Rated",
        src:
          "data:image/png;base64,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",
      },
      {
        label: "Upcoming",
        src:
          "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAABmJLR0QA/wD/AP+gvaeTAAADW0lEQVR4nO3cT08TQRzG8S8oVZC2GBNj8BUoV++eTPQC8aX4QhQSYnwL+hKMN8/eFL2rF0KitPwRBcHD7JLt7La73XZ3fnWfT7KUttv5TedpZwmTDIiIiIiIiIiIiMyGOe9+G3gGPAIWgT/AEXAGHAAXwH50bg84Bw6BU+AXcJJ4zV+gH537M7rtR4/HfgPHGf1K1qnKCun3D7AEXEvcvwJ0ot9vRred6PEbQAu4jhuvBWAZmAe6Xp02cDXR/jHwDtjCjS14HboFvAful3hzdTrAfUCKiAfIsk/AQ+CH/8Qr3CdTR/3HyziE5DdkF7jtpyS12AXuwGAgF95JD3Bz3RJu7mtH569Ez3dxc+UybmpYxM2lLdzcOmrujSXnWl8851bhFHfty7LP4FiMuhYe4a6ZJ7hraNzuOe4am2wvnmqPcdfOD17ducsfET+QrAueBfGHpIh4wCzKHO9ZDOR/kTne8wE6IiMoEGMUiDEKxBgFYowCMUaBGKNAjFEgxigQYxSIMQrEGAVijAIxRoEYo0CMUSDGKBBjFIgxCsQYBWKMAjFGgRijQIxRIMYoEGMUiDEKxBgFYowCMUaBGKNAjFEgxigQYxSIMQrEGAVijAIxRoEYU0cga8AmbpOVQ8bfB+Qweu0Lym2ME7p+aX5HJtUCtnHbSUxrk5Yz3HZGCzNQP0/ueE8zkBZuL6iqds95y+hBCV2/iFoD2c5ob9rHluH6RdQWyBrpaWIHWMft8DOuNrABfPbaPAXuGaxfVG2BbJIejM7IVxTTBb54bT83WL+o3PHuZZxU5PDteM9vTNBp31Ov7Y8G65cZw8z9Jd+UbMzX954vM00M0/Ha7mecE7p+mTF8nVXsLrBXorG8Dk3brNXPO/aA1WHFVnFpjTN9jdvhSc1a/WFHDzfWA2FUsWuc38lp18hrP3T9ieh/WcZUtetnUhXTxizVH4u+IcZUEcj3Ctoc5pvB+uY8wXW0zN/j4xxfgccG64uIiJgVek266fUvhV6Tbnr9VGeavCYeun5K6DXpptcfEHpNuun1U0KvSTe9fkroNemm108JvSbd6PpZq10XBc6ZRF77ja6v9RBjFIgxCsSYImvq/pxXt0bV1zfEmKxAQq9JN71+Sug16abXFxEREZGp+wf78k7F+VifoAAAAABJRU5ErkJggg==",
      },
    ],
    sidegenres: [
      {
        label: "Action",
        src:
          "data:image/png;base64,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",
      },
      {
        label: "Adventure",
        src:
          "data:image/png;base64,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",
      },
      {
        label: "Animation",
        src:
          "data:image/png;base64,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",
      },
      {
        label: "Comedy",
        src:
          "data:image/png;base64,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",
      },
      {
        label: "Crime",
        src:
          "data:image/png;base64,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",
      },
      {
        label: "Documentary",
        src:
          "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAABmJLR0QA/wD/AP+gvaeTAAAF8klEQVR4nO2dS2xVRRjHfy21XVgeEosRKYaQaMvCqMhCpEoxihhd+AgrtppW2LuSsNFIrAvCTmOMcacQH4CoQbAFkUILWkzcUUElJholQoIGeutiTsI9M3POPY+5c6be75fM4t47Z77//f7nOTN3LgiCIAiCIAiCIPilzUEbK4CNwADQDywHFgDXgD+A34HvgVHgCPCzg5g2eoFBYD1wD9AD3ArcBPwNXAB+BI4CnwM/NUlHJbQDm1FfrgbMZiw1VDKeitpwoeNp4IsCOsaA5x3pqJRB4Aeyf/mkMgE8UELHGuC0Ax1ngUdK6KiMLmA3+fbERuU68AYwL4eODmAk2taVjhqwC+jMoaNSFgPHSf5Ck8B21Pm7D7g5Kn2oI2p7VCdp+wPA/Aw6FgAHm6jjGHBLztx4ZzEwhX2v+hC4O0dbfcAe7EfZKaA7Zdv52JPpWscU6jsHSRf2I+Mc8GCJdtcC05Z292M/fXWgjiJfOo4R6OlrN6bYUdTtZFl6UHc6evuvWeq+XoGOXQ7adsog5iE9its9pxMzGdeAe+vq3Be951tHjYDuvtoxb23P4WaP1OnBPG2Mox5a24CTFeqYIpDnlM2Ye0uZc3UjHsI8ZTwKPBaAjueaGC8zR4mL+sBDzL1azH2oi3zVOo54iJnKCuLXjhr5bimL0k88ETNRqVpHDbjTQ9xEhjVBEx5jn8E8ZYSg4wVfgW0XrHXa6099CIn4JOWzKnU87CuwzZB+7fWYDyEZYlWpQ89J07AZslx7fdGHkIhfUz6rUoeeE6/8S/z8mda/5Jpukq8hVer4x1dg2xEyq712MaqYlbSHsCp16DnxFhjUcGc9t/sQErE05bMqdVzyFdhmyC/a6zt8CIlIM6RKHWnXNqfYDDmrvfZ2y0d6Z16VOqY8xjYYIn5BO+0x9nckX9Sr1PGix9gGvZhdJ30e4q4ingRb10kVOmqkn0q98DVxUXs8xPxYi7kPc5SwCh2HPMRsyLOYe8naJsYbwDxFbQSeCEDHM02Ml5l2zAkF06hBHNcsQc0irI91ghsDVOMV6pggkAEqUHca+hDuGG6HTrswx16uA/fX1VmNOQfLh44ZzI7WyhnBPITHcLOHLsFMwixqQoPOzgp07HTQtnM6USNmuthp1HBnUQaA85Z2D2KfBjQPNSfYl46vCHQaEMBCkufQ7iVf1/Qq4KOEtsaBRSnbLsK8njRDxyRqhmTQLAQOk/zQdgbYAWxAPSt0R6Uvem8H6aOBh8jWm9sd1W2WjsMEaEYnsA11p3OFZPGtUq4A3wJbqeA0thQ3U/z/r2USj73OnYgZWcoE6ldZTWdbBV9urpbhgjnOxQkt6H78jkGEyjLMPrXjPgJf1oIu8xF0jtBLPDf6qKoz6sepZ1M+EzzlJ5iOM0EhhvjhNtQPgM4TH3SrLwYNK7Q4RfOzAbWAQqM7N2cBW4Ui+XkSuGrZVgxxQN78PI45C1QMcUie/KxG3RrX158BXkENhmVqTwxJJ2t+7gJ+0+rWgJfytieGpJMlPytRsxz1ui8XaU8MSadRftajloDS671asD0xpAFZL8715V2Sn+jFkJLkNeM90lc5EkNKktWIGmrJqUa9IGJISRoZ8Seqmz7rchzWfHe409tySG9vKyCGBIYYEhhiSGCIIYEhhgSGGBIYYkhgiCGBIYYEhhgSGGJIYIghgSGGBIYYEhhiSHH0AaZLwJfApmYFEOLkGU9/i8aDfzKEW5K8kxzeJ/0MJIaUpMg0oJEc7eWv0OI0ys867BPlthRsTwxpQJb8rEQt+Fxf7yrqL/5ytyeGpJM1P2swfxNyEWVWrvbEkHTy5GeLpf4F4utviSElyZufNy3bpJXSAVuNvPlpA96xbCeGOKJIfjqAty3biiEOKJOfTah/tP7L0k5ie/pv4mRpjRt4W1qjHn3xmQOIKaDM+Ix4brwsPrOV5MNJSrwMFcxxLjpJ/2trKaqcxNMCZqCWr5to8heay+UUfv9YBlDuDwPfYK6h1YrlcpSLITweGYIgCIIgCIJL/gMQ40o2WmE9twAAAABJRU5ErkJggg==",
      },
      {
        label: "Drama",
        src:
          "data:image/png;base64,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",
      },
      {
        label: "Family",
        src:
          "data:image/png;base64,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",
      },
    ],
  }),
  methods: {
    search() {
      if (this.searchTerm === "") {
        return;
      }
      fetch(`${searchURL}${this.searchTerm}`)
        .then((val) => val.json())
        .then((movies) => {
          console.log("movies", movies);
          this.imgs = this.parseImgResponse(movies);
        });
    },
    parseImgResponse(movies) {
      return movies.results.reduce((acc, movie) => {
        if (!movie.poster_path) {
          return acc;
        }
        acc.push({
          poster: `${bg}${movie.poster_path}`,
          date: movie.release_date,
          title: movie.title,
        });
        return acc;
      }, []);
    },
  },
  mounted() {
    fetch(popURL)
      .then((info) => info.json())
      .then((movies) => {
        console.log(movies);
        this.imgs = this.parseImgResponse(movies);
      });
  },
};
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
</style>
