<template>
  <div class="interests-container">
    <div class="interests-header">
      <h5><strong>Genesis Belmonte's Interests</strong></h5>
    </div>
    <interests-columns
      v-for="(column, index) in columns"
      :key="index"
      :columnTitle="column.title"
      :columnInformation="column.information"
    />
  </div>
</template>

<script>
import InterestsColumns from "./InterestsColumns.vue";
export default {
  components: {
    InterestsColumns,
  },
  data: () => ({
    columns: [
      {
        title: "General",
        information:
          "Working on personal projects, watching shows, playing Stardew Valley when I can, a LOT of interesting Youtube videos, more in the educational realm.",
      },
      {
        title: "Music",
        information:
          "Rezz, Beyonce, ABBA, Prince, Tiesto, Elton John, Ariana Grande, Mylie Cyrus, SZA",
      },
      {
        title: "Television",
        information:
          "Parks & Recreation, The Office, Community, What we do in the Shadows, Bob's Burgers, American Dad, Modern Family",
      },
      {
        title: "Books",
        information:
          "The Martian, The Hunger Games, Ready Player One, Angels & Demons, Uglies, Hitchhiker's Guide to the Galaxy, ",
      },
      {
        title: "Heroes",
        information: "Captain Janeway, Judge Judy",
      },
    ],
  }),
};
</script>
