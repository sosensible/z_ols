<template>
  <div class="mb-3">
    <label :for="id" class="form-label">{{ label }}</label>
    <input
      :id="id"
      class="form-control"
      :value="modelValue"
      @input="$emit('update:modelValue', $event.target.value)"
      :type="type"
    />
  </div>
</template>
<script>
export default {
  emits: ["update:modelValue"],
  props: {
    label: String,
    id: String,
    modelValue: String,
    type: String,
  },
};
</script>
