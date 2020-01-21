<template>
  <div>
    <header class="bg-gray-900 p-4 pb-5">
      <div class="flex justify-between items-center">
        <button>
          <svg class="w-5 h-5 fill-current text-white" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" /></svg>
        </button>
        <a href="#">
          <svg class="w-8 h-8 fill-current text-white" viewBox="0 0 16 16" version="1.1" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
        </a>
        <a href="#">
          <svg class="w-5 h-5 text-white fill-current" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M8.0274 2.3318C5.6827 3.1477 4 5.3773 4 8v6l-3 2v1h18v-1l-3-2V8c0-2.6227-1.6827-4.8523-4.0274-5.6682C11.9906 2.2238 12 2.113 12 2c0-1.1046-.8954-2-2-2S8 .8954 8 2c0 .113.0094.2239.0274.3318zM12 18c0 1.1046-.8954 2-2 2s-2-.8954-2-2h4z" /></svg>
        </a>
      </div>
      <div class="flex justify-center align-center pt-4">
        <a class="px-2 text-white text-sm font-semibold" href="#">Dashboard</a>
        <a class="ml-1 px-2 text-gray-500 text-sm" href="#">Pull requests</a>
        <a class="ml-1 px-2 text-gray-500 text-sm" href="#">Issues</a>
      </div>
    </header>

    <nav class="w-full flex">
      <a class="block text-center pt-2 pb-3 w-1/2 no-underline text-sm font-semibold bg-white" href="#">Overview</a>
      <a class="border block text-center pt-2 pb-3 w-1/2 no-underline text-sm font-semibold text-blue-600 bg-gray-100" href="#">Explore repositories</a>
    </nav>

    <div class="p-4">

      <input class="px-2 py-1 bg-gray-100 border border-gray-400 focus:outline-none focus:shadow-outline rounded block w-full shadow-inner" placeholder="Search GitHub" />

      <div class="mt-4 border border-gray-400 rounded overflow-hidden">
        <div class="px-3 py-2 bg-gray-100 font-semibold text-sm">Recent activity</div>
        <div class="p-3 flex items-start border-t border-gray-400">
          <svg class="w-4 h-4 fill-current text-green-500" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M2.929 17.071c3.9052 3.9053 10.2368 3.9053 14.142 0 3.9053-3.9052 3.9053-10.2368 0-14.142-3.9052-3.9053-10.2368-3.9053-14.142 0-3.9053 3.9052-3.9053 10.2368 0 14.142zm12.7279-1.4141c3.1241-3.1242 3.1241-8.1896 0-11.3138-3.1242-3.1241-8.1896-3.1241-11.3138 0-3.1241 3.1242-3.1241 8.1896 0 11.3138 3.1242 3.1241 8.1896 3.1241 11.3138 0zM9 5h2v6H9V5zm0 8h2v2H9v-2z" fill-rule="evenodd"/></svg>
          <div class="-mt-2 ml-1">
            <a class="font-bold text-sm" href="#">error pas buka list-rak.php</a>
            <div class="break-words">
              <img class="inline-block rounded w-4 h-4 object-cover" src="https://avatars1.githubusercontent.com/u/10344542?s=40&v=4" alt="profile" />
              <img class="inline-block ml-1 rounded w-4 h-4 object-cover" src="https://avatars3.githubusercontent.com/u/56142220?s=40&v=4" alt="profile" />
              <span class="inline-block mx-1">·</span>
              <a class="text-gray-700 text-xs hover:text-blue-600" href="#">YusufAdiNugroho1/perpus</a>
              <span class="inline-block mx-1">·</span>
              <span class="text-gray-700 text-xs">Someone commented</span>
              <a class="inline-block ml-1 text-xs text-gray-700 hover:text-blue-600" href="#">10 days ago</a>
            </div>
          </div>
        </div>
      </div>

      <div class="mt-4 border border-gray-400 rounded overflow-hidden">
        <div class="px-3 py-2 bg-gray-100 font-semibold text-sm">Repositories you contribute to</div>
        <div>
          <a v-for="item in contributions" :key="item.repo" class="flex items-center p-3 border-t border-gray-400" href="#">
            <svg class="w-3 h-4 fill-current text-gray-900" viewBox="0 0 12 16" version="1.1" aria-hidden="true"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"></path></svg>
            <span class="ml-2 flex-grow text-sm font-bold text-blue-600">{{ item.repo }}</span>
            <div class="flex items-center text-gray-900">
              <span class="text-xs">{{ item.stars }}</span>
              <svg class="ml-1 w-4 h-4 fill-current" viewBox="0 0 14 16" version="1.1" aria-hidden="true"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74L14 6z"></path></svg>
            </div>
          </a>
        </div>
      </div>

      <div class="mt-4 border border-gray-400 rounded overflow-hidden">
        <div class="px-3 py-2 bg-gray-100 font-semibold text-sm">Starred repositories</div>
        <div>
          <a v-for="item in starredRepos" :key="item.repo" class="flex items-center p-3 border-t border-gray-400" href="#">
            <svg class="w-3 h-4 fill-current text-gray-900" viewBox="0 0 12 16" version="1.1" aria-hidden="true"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"></path></svg>
            <span class="ml-2 flex-grow text-sm font-bold text-blue-600">{{ item.repo }}</span>
            <div class="flex items-center text-gray-900">
              <span class="text-xs">{{ item.stars }}</span>
              <svg class="ml-1 w-4 h-4 fill-current" viewBox="0 0 14 16" version="1.1" aria-hidden="true"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74L14 6z"></path></svg>
            </div>
          </a>
        </div>
      </div>

      <div class="mt-4 border border-gray-400 rounded overflow-hidden">
        <div class="px-3 py-2 bg-gray-100 font-semibold text-sm">Teams you belong to</div>
        <div>
          <a v-for="item in teams" :key="item.repo" class="flex items-center p-3 border-t border-gray-400" href="#">
            <svg class="w-4 h-4 fill-current text-gray-900" viewBox="0 0 14 16" version="1.1" aria-hidden="true"><path fill-rule="evenodd" d="M4.5 6l-.5.5v5l.5.5h2l.5-.5v-5L6.5 6h-2zM6 11H5V7h1v4zm6.27-7.25C12.05 2.37 11.96 1.12 12 0H9.02c0 .27-.13.48-.39.69-.25.2-.63.3-1.13.3-.5 0-.88-.09-1.13-.3-.23-.2-.36-.42-.36-.69H3c.05 1.13-.03 2.38-.25 3.75C2.55 5.13 1.95 5.88 1 6v9c.02.27.11.48.31.69.2.21.42.3.69.31h11c.27-.02.48-.11.69-.31.21-.2.3-.42.31-.69V6c-.95-.13-1.53-.88-1.75-2.25h.02zM13 15H2V7c.89-.5 1.48-1.25 1.72-2.25S4.03 2.5 4 1h1c-.02.78.16 1.47.52 2.06.36.58 1.02.89 2 .94.98-.02 1.64-.33 2-.94.36-.59.5-1.28.48-2.06h1c.02 1.42.13 2.55.33 3.38.2.81.69 2 1.67 2.63v8V15zM8.5 6l-.5.5v5l.5.5h2l.5-.5v-5l-.5-.5h-2zm1.5 5H9V7h1v4z"></path></svg>
            <span class="ml-2 flex-grow text-sm font-bold text-blue-600">{{ item.team }}</span>
          </a>
        </div>
      </div>

    </div>

    <footer class="px-4 py-3 flex flex-between items-center bg-gray-100 border-t border-gray-400">
      <a class="flex-grow" href="#">
        <svg class="w-8 h-8 fill-current text-gray-500" viewBox="0 0 16 16" version="1.1" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
      </a>
      <a class="text-sm text-gray-500" href="#">Desktop version</a>
      <a class="text-sm ml-4 text-gray-500" href="#">Sign out</a>
    </footer>

  </div>
</template>

<script>
export default {
  data() {
    return {
      teams: [
        {
          team: 'ajaroid/ajaro'
        }
      ],
      contributions: [
        {
          repo: 'pirey/dotfiles',
          stars: 6
        },
        {
          repo: 'pirey/alokasi',
          stars: 0
        },
        {
          repo: 'pirey/portofolio',
          stars: 0
        },
        {
          repo: 'pirey/workshop-pos-client',
          stars: 0
        },
        {
          repo: 'pirey/react-starter',
          stars: 0
        },
        {
          repo: 'pirey/code-generator',
          stars: 1
        },
      ],
      starredRepos: [
        {
          repo: 'adonisjs/adonis-lucid',
          stars: '4,004',
        },

        {
          repo: 'terser/terser',
          stars: '4,560'
        },
        {
          repo: 'kognise/water.css',
          stars: '399',
        },
        {
          repo: 'brammool/vim9',
          stars: '2,573',
        },
        {
          repo: 'asciimoo/drawille',
          stars: '5,283',
        },
        {
          repo: 'gobuffalo/buffalo',
          stars: '1,072',
        },
        {
          repo: 'dyng/ctrlsf.vim',
          stars: '124',
        },
        {
          repo: 'othree/es.next.syntax.vim',
          stars: '249',
        },
        {
          repo: 'skywind3000/vim-quickui',
          stars: '136',
        },
        {
          repo: 'utsmannn/Kemana',
          stars: '136'
        }
      ]
    }
  }
}
</script>
