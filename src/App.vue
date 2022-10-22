<template>
<div id="app"> 
  <div class="container grid-xs py-2">

    <img class="img-responsive" src="@/assets/lista.png" alt="CoffeTagTodo">

    <form>
      <div class="input-group">
          <input type="text" class="form-input" placeholder="adicionar uma tarefa">
          <button class="btn btn-success input-group-btn"> adicionar <i class="icon icon-arrow-right"></i></button>
      </div>
    </form>

    <ul class="step">
      <li class="step-item active">
        <a href="#" class="tooltip" data-tooltip="Step 1">Step 1</a>
        </li>
      <li class="step-item ">
        <a href="#" class="tooltip" data-tooltip="Step 2">Step 2</a>
      </li>
      <li class="step-item">
        <a href="#" class="tooltip" data-tooltip="Step 3">Step 3</a>
      </li>
      <li class="step-item ">
        <a href="#" class="tooltip" data-tooltip="Step 4">Step 4</a>
      </li>
  </ul>

  </div>
</div>
 
  
</template>

<script>


export default {
  name: 'App',

}
</script>

<style scoped>
  img {
    max-width: 90px;
    margin:0 auto;
  }

  .input-group{
    margin-top: 3vh;
  }
</style>
