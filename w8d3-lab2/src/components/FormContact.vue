<template>
  <div>
    <div class="formulario">
    <input class="form-element" v-model="name" placeholder="Nombre" /><br>
    <input class="form-element" v-model="mail" placeholder="e-mail" /><br>
    <textarea v-model="message" placeholder="escriba aquí su mensaje"></textarea
    ><br>
    <p>Seleccione su talla</p>
    <input type="radio" value="L" v-model="size" />
    <label for="L">L</label>
    <br>
    <input type="radio" value="M" v-model="size" />
    <label for="M">M</label>
    <br>
    <input type="radio" value="S" v-model="size" />
    <label for="S">S</label>
    <p>Eliga un color</p>
    <select v-model="color">
    <option disabled value="">Seleccione un color</option>
    <option>Azul</option>
    <option>Rojo</option>
    <option>Verde</option>
    </select><br>
    <input type="checkbox" v-model="checkedInfo" />
    <label>Envolver para regalo</label><br>
    </div>

    <p>Mi nombre és: {{ name }}</p>
    <p>Mi e-mail és: {{ mail }}</p>
    <p>Su mensaje és: {{ message }}</p>
    <p>Talla seleccionada: {{ size }}</p>
    <p>Color seleccionado: {{ color }}</p>
    <p>Envolver para regalo: {{ checkedInfo }}</p>
  </div>
</template>

<script>
export default {
  name: "FormContact",
  data() {
    return {
      name: "",
      mail: "",
      message: "",
      checkedInfo: "",
      size: "",
      color: "",
    };
  },
};
</script>

<style>
.formulario{
    width:300px;
	padding:16px;
	border-radius:10px;
	background-color:rgb(170, 240, 237);
}

.form-element {
    width: 90%;
	margin-top:5px;
   padding:5px;
}

textarea {
    width: 90%;
	margin-top:5px;
    padding:5px;
}

select {
    width: 90%;
	margin-top:2px;
    margin-bottom: 10px;
    padding:5px;
}
</style>
