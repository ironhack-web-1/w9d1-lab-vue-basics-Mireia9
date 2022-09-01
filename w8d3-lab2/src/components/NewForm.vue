<template>
  <div>
    <div class="formulario">
      <input :type="type" :name="modelValue" :placeholder="placeholder" 
      @input="$emit('update:modelValue', $event.target.value)"
      />
    </div>
  </div>
</template>

<script>

export default {
  name: "NewForm",
  data() {
    return {

    };
  },
  props: {
    type: {
      type: String,
      required: false,
      default: "text",
    },
    placeholder: String,
    modelValue: {
      required: true,
      default: "Nombre desconocido",
    }
  }
};
</script>

<style scoped>
.formulario {
  width: 300px;
  padding: 16px;
  border-radius: 10px;
  background-color: rgb(229, 219, 26);
}

.form-element {
  width: 90%;
  margin-top: 5px;
  padding: 5px;
}
</style>
