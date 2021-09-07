<template>
  <div class="skill-wrap flex flex-col">
    <div class="skill-content">
      <slot></slot>
    </div>
    <div
      v-if="hasRating"
      class="skill-rating text-right flex flex-col"
    >
      <RatingDots :value="rating ?? 0"></RatingDots>
      <span class="text-gray-700">
        {{ computedSkillRatingLabel }}
      </span>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { computed } from "vue";
import RatingDots from "./RatingDots.vue";
import { isString, isUndefined } from "lodash-es";

const props = defineProps({
  rating: {
    type: Number,
    required: false,
    default: undefined,
    validator: function (value: number) {
      return value >= 0 && value <= 5;
    },
  },
  ratingLabel: {
    type: String,
    required: false,
    default: undefined,
  },
});

const defaultRatingLabel = () => {
  switch (props.rating) {
    case 0:
      return 'Poor';
    case 1:
      return 'Low';
    case 2:
      return 'Sufficient';
    case 3:
      return 'Good';
    case 4:
      return 'Very Good';
    case 5:
    default:
      return 'Excellent';
  }
}

const computedSkillRatingLabel = computed(() => {
  return isString(props.ratingLabel)
    ? props.rating
    : defaultRatingLabel();
});

const hasRating = computed(() => {
  return !isUndefined(props.rating)
})
</script>
