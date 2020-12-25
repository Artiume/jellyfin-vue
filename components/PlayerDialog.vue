<script lang="ts">
import Vue from 'vue';
import { VDialog } from 'vuetify/lib';

export default Vue.extend({
  extends: VDialog,
  methods: {
    // Copy of https://github.com/vuetifyjs/vuetify/blob/master/packages/vuetify/src/mixins/overlayable/index.ts#L129
    // A block preventing events on the overlay has been removed.
    shouldScroll() {
      return true;
    }
  }
});
</script>
