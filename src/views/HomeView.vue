<template>
  <div id="homepage" class="row">
    <div class="col">
      <h5><b>Genesis Belmonte</b></h5>
      <div class="col d-inline-flex">
        <img
          id="profile-pic"
          class="d-inline"
          src="../assets/profile-pic.jpeg"
        />
        <div class="px-2 w-25">
          <small
            >"Don't cry because it's over smile because it happened."</small
          >
          <br /><br />
          <small class="p-4">
            Female<br />30 years old<br />Pueblo West<br />COLORADO<br />United
            States
          </small>
          <br /><br />
          <small class="profile-pic-text"> Last Login:<br /> </small>
          <small>{{ currentDate }}</small>
        </div>
        <!-- <div> -->
        <!-- </div> -->
      </div>
      <div id="under-photo-section">
        <p>
          <strong>Mood: </strong>productive 😁 <br />View My:
          <strong>
            <a class="pics-and-video-links" href="/pics">Pics</a></strong
          >
          |
          <strong>
            <a class="pics-and-video-links" href="/videos">Videos</a>
          </strong>
        </p>
      </div>
      <div class="contacting-genesis-container">
        <div class="contacting-genesis-header">
          <h5><strong>Contacting Genesis</strong></h5>
        </div>
        <div class="container">
          <div class="row">
            <div class="col contacting-options-container">
              <a class="contacting-options-container-links" href="#"
                ><p>Send Message</p></a
              >
              <a class="contacting-options-container-links" href="#">
                <p>Add to Friends</p>
              </a>
              <a class="contacting-options-container-links" href="">
                <p>Instant Message</p>
              </a>
              <a class="contacting-options-container-links" href="">
                <p>Add to Group</p>
              </a>
            </div>
            <div class="col contacting-options-container">
              <a class="contacting-options-container-links" href="#">
                <p>Forward to a Friend</p>
              </a>
              <a class="contacting-options-container-links" href="#">
                <p>Add to Favorites</p>
              </a>
              <a class="contacting-options-container-links" href="#">
                <p>Block user</p>
              </a>
              <a class="contacting-options-container-links" href="#">
                <p>Rank user</p>
              </a>
            </div>
          </div>
        </div>
      </div>
      <div id="myface-url-section" class="mb-4 mt-4">
        <strong>Myface URL:</strong><br />
        https://www.myface.com/genesisbelmonte
      </div>
      <div class="interests-container">
        <div class="interests-header">
          <h5><strong>Genesis Belmonte's Interests</strong></h5>
        </div>
        <div class="row mb-2 g-2">
          <div class="col">
            <div class="interests-left-col">
              <h5>General</h5>
            </div>
          </div>
          <div class="col">
            <div class="interests-right-col">
              <p>
                Fusce sit amet pellentesque erat. Mauris rutrum fringilla ante.
                Morbi quis arcu rhoncus, tincidunt nisi eu, venenatis dui. Nulla
                sollicitudin blandit lorem, in fringilla diam mattis id.
                Praesent finibus lectus quis risus ultrices elementum. Nullam
                finibus enim nec mauris ultricies bibendum.
              </p>
            </div>
          </div>
        </div>
        <div class="row mb-2 g-2">
          <div class="col">
            <div class="interests-left-col">
              <h5>Music</h5>
            </div>
          </div>
          <div class="col">
            <div class="interests-right-col">
              <p>
                Rezz, Beyonce, ABBA, Prince, Tiesto, Elton John, Ariana Grande,
                Mylie Cyrus, SZA
              </p>
            </div>
          </div>
        </div>
        <div class="row mb-2 g-2">
          <div class="col">
            <div class="interests-left-col">
              <h5>Television</h5>
            </div>
          </div>
          <div class="col">
            <div class="interests-right-col">
              <p>
                Integer ac iaculis felis. Aenean condimentum, metus id efficitur
                aliquet, lorem tortor molestie diam, at pretium ipsum nunc eget
                tortor. Maecenas luctus nisl purus, quis dictum ex finibus
                congue. Nunc sed felis tellus. Cras vitae ullamcorper nisl.
              </p>
            </div>
          </div>
        </div>
        <div class="row mb-2 g-2">
          <div class="col">
            <div class="interests-left-col">
              <h5>Books</h5>
            </div>
          </div>
          <div class="col">
            <div class="interests-right-col">
              <p>
                Phasellus lectus lectus, fermentum non viverra et, gravida et
                odio. Nulla odio nunc, blandit ac erat quis, efficitur
                vestibulum ex. Aliquam sagittis sem eget tincidunt cursus.
              </p>
            </div>
          </div>
        </div>
        <div class="row mb-2 g-2">
          <div class="col">
            <div class="interests-left-col">
              <h5>Heroes</h5>
            </div>
          </div>
          <div class="col">
            <div class="interests-right-col">
              <p>Captain Janeway, Judge Judy</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col">
      <div id="extended-network-banner">
        <h4>Genesis is in your extended network.</h4>
      </div>
      <p class="mt-4">
        <strong>
          Genesis Belmonte's Latest Blog Entry [<a
            class="blog-page-link"
            href="#"
            >Subscribe to this Blog</a
          >]
        </strong>
      </p>
      <p>
        If a duckling is a little duck, then a dumpling is a little dump. (<a
          class="blog-page-link"
          href="#"
          >view more</a
        >)
      </p>
      <p>
        Babies are annoying. I know. I have one. (<a
          class="blog-page-link"
          href="#"
          >view more</a
        >)
      </p>
      <h5 class="blurbs-header">Genesis Belmonte's Blurbs</h5>
      <h5 class="blurbs-header-title">About me:</h5>
      <p>
        Donec elementum non dolor id posuere. Maecenas tortor lorem, tempor
        vitae leo id, ultricies mollis diam. Pellentesque habitant morbi
        tristique senectus et netus et malesuada fames ac turpis egestas. In
        metus lorem, semper eu facilisis et, finibus in urna. Vestibulum ante
        ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae;
        Curabitur iaculis, massa at placerat dictum, lorem libero viverra erat,
        id convallis tellus est nec dolor. Phasellus non sapien at libero
        rhoncus ultricies vel eu sapien. Suspendisse commodo lorem nisi, nec
        lobortis turpis laoreet ac. Pellentesque at nisl nec nulla molestie
        pharetra. Pellentesque tempus nunc nec fringilla feugiat. Aenean nec
        aliquam urna. Nunc et libero dignissim, pretium turpis lobortis, dapibus
        libero. Donec elementum dapibus lacinia.
      </p>
      <h5 class="blurbs-header-title">Who I'd like to me:</h5>
      <p>
        Praesent vitae velit libero. Ut pharetra bibendum metus nec eleifend.
        Donec a mi at ex vestibulum dictum eget sed dui. Donec a est fringilla,
        volutpat ligula nec, venenatis eros. In arcu urna, malesuada quis dui
        sit amet, interdum mollis odio. Integer in risus sapien. Praesent
        sollicitudin varius ipsum, nec malesuada felis maximus sed.
      </p>
      <h5 class="blurbs-header">Genesis Belmonte's Friend Space:</h5>
      <p>
        <strong
          >Genesis Belmonte has
          <span class="blurbs-header-title">a gajillion</span> friends.</strong
        >
      </p>
      <div class="row g-0">
        <div class="col">
          <p class="myface-friend">
            Friend<br />
            <img src="https://placekitten.com/200/300" />
          </p>
        </div>
        <div class="col">
          <p class="myface-friend">
            Friend<br />
            <img src="https://placekitten.com/100/100" />
          </p>
        </div>
        <div class="col">
          <p class="myface-friend">
            Friend<br />
            <img src="https://placekitten.com/200/150" />
          </p>
        </div>
        <div class="col">
          <p class="myface-friend">
            Friend<br />
            <img src="https://placekitten.com/200/250" />
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  computed: {
    currentDate() {
      var currentDateWithFormat = new Date()
        .toJSON()
        .slice(0, 10)
        .replace(/-/g, "/");
      return currentDateWithFormat.toString();
    },
  },
};
</script>
