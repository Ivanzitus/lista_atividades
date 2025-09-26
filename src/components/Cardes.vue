<template>
    <div class="card card-border bg-base-100 w-96">
  <div class="card-body">
    <h2 class="card-title">{{tarefa.nome}}</h2>
    <p>{{tarefa.descricao}}</p>
    <div class="card-actions justify-end">
      <button class="btn btn-primary">{{tarefa.propriedade}}</button>
    </div>
  </div>
</div>
</template>

<script>
export default{
    name:"Card",
    props:{
        tarefa:{
            id:Number,
            nome:String,
            descricao:String,
            propriedade:String,
            status:boolean,
        }
    }
}
</script>