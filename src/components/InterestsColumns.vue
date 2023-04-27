<template>
  <div class="row mb-2 g-2">
    <div class="col">
      <div class="interests-left-col">
        <h5>{{ columnTitle }}</h5>
      </div>
    </div>
    <div class="col">
      <div class="interests-right-col">
        <p>
          {{ columnInformation }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    columnTitle: String,
    columnInformation: String,
  },
  data: () => ({}),
};
</script>
