 <template>
 <div
    :class="[
      foo ? '' : bar(),
      'foo',
    ]"
  >
  Hello World
</div>
</template>

<script setup lang="ts">
import {
  bar,
} from "@/utils";


defineProps({
  foo: { type: Boolean, required: true },
});
</script>