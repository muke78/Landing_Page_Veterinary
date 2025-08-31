<script setup lang="ts">
import { ref } from "vue"
import { Button } from "@/components/ui/button"

const count = ref(0)

const incrementCount = () => {
  count.value++
}

</script>

<template>
  <div>
    <Button variant="secondary" @click="incrementCount">
      Count is: {{ count }}
    </Button>
  </div>
</template>