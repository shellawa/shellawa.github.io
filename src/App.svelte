<script>
  import Header from "./lib/Header.svelte";
  import Link from "./lib/Link.svelte";
  const info = {
    header: {
      name: "Shella",
      bio: "awa",
      avatarUrl: "futaribeya_kasumi_1.png",
    },
    links: [
      {
        name: "osu!",
        icon: "osu.png",
        link: "https://osu.ppy.sh/users/13368266",
      },
      {
        name: "Facebook",
        icon: "facebook.png",
        link: "https://www.facebook.com/shellawawawa/"
      },
      {
        name: "Reddit",
        icon: "reddit.png",
        link: "https://www.reddit.com/user/allehS"
      },
      {
        name: "Asymmetry🌿#3510",
        icon: "discord.png",
        link: "https://discord.com/users/749117124831608853"
      },
      {
        name: "Github",
        icon: "github.png",
        link: "https://github.com/Hiyoriii"
      },
      {
        name: "Steam",
        icon: "steam.png",
        link: "https://steamcommunity.com/id/allehS"
      },
      {
        name: "MyAnimeList",
        icon: "mal.png",
        link: "https://myanimelist.net/profile/shellasinn"
      },
      {
        name: "ln.hako",
        icon: "hako.png",
        link: "https://ln.hako.vn/thanh-vien/119235"
      }
    ],
  };
</script>

<div class="body">
  <div class="container">
    <Header data={info.header} />
    <div class="linksContainer">
      {#each info.links as linkData}
        <Link data={linkData} />
      {/each}
    </div>
  </div>
</div>

<style>
  .body {
    min-height: 100vh;
    background-color: #36393f;
  }
  @media screen and (min-width: 768px) {
    .body {
      display: flex;
      justify-content: center;
    }
  }
  .container {
    width: 100%;
    height: 100%;
  }
  @media screen and (min-width: 0) {
    .container {
      margin: 0;
    }
  }
  @media screen and (min-width: 768px) {
    .container {
      max-width: 60rem;
      padding: 3rem;
      border-radius: 3rem;
      margin-top: 3rem;
    }
  }
  @media screen and (min-width: 900px) {
    .container {
      max-width: 75rem;
    }
  }
  @media screen and (min-width: 1260px) {
    .container {
      max-width: 80rem;
    }
  }
  .linksContainer {
    margin-top: 2rem;
    padding: 1rem 0;
  }
  @media screen and (min-width: 0) {
    .linksContainer {
      padding-bottom: 15rem;
    }
  }
  @media screen and (min-width: 768px) {
    .linksContainer {
      padding-bottom: 3rem;
    }
  }
</style>
