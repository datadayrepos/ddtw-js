<template>
  <div class="vp-raw flex flex-wrap items-center gap-2">
    <DdtwButton
      :disabled="loading"
      :loading="loading"
      gradient="purple-blue"
      outline
      size="xs"
      @click="loading = !loading"
    >
      Click me
    </DdtwButton>
    <DdtwButton
      :loading="loading"
      gradient="red-yellow"
      size="sm"
      @click="loading = !loading"
    >
      Click me
    </DdtwButton>
    <DdtwButton
      :loading="loading"
      color="default"
      loading-position="suffix"
      outline
      @click="loading = !loading"
    >
      Click me
      <template #suffix>
        <svg
          class="w-5 h-5"
          fill="currentColor"
          viewBox="0 0 20 20"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            clip-rule="evenodd"
            d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
            fill-rule="evenodd"
          />
        </svg>
      </template>
    </DdtwButton>
    <DdtwButton
      :loading="loading"
      gradient="green-blue"
      size="lg"
      @click="loading = !loading"
    >
      Click me
    </DdtwButton>
    <DdtwButton
      :loading="loading"
      gradient="pink"
      size="xl"
      @click="loading = !loading"
    >
      Click me
    </DdtwButton>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
import { DdtwButton } from '../../../../src/index'

const loading = ref(false)
</script>
