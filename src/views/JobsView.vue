<template>
  <div>
    <list-item></list-item>
    <!-- <ul class="job-list">
      <li v-for="job in this.$store.state.jobs" v-bind:key="job.id" class="post">
        <div class="points">
           {{ job.points || 0 }}
        </div>
        <div>
          <p class="job-title">
            <a :href="job.url">
              {{ job.title }}
            </a>
          </p>
          <small class="link-text">
            {{ job.time_ago }} by
            <a :href="job.url">
              {{ job.domain }}
            </a>
          </small>
        </div>
      </li>
    </ul> -->
  </div>
</template>

<script>
import ListItem from '../components/ListItem.vue';
import ListMixin from '../mixins/ListMixin.js';
// import bus from '../utils/bus.js';

export default {
  components: { ListItem },
  mixins: [ListMixin],
}
</script>
