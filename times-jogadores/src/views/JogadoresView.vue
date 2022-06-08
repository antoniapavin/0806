<script>
export default {
  data() {
    return {
      jogadores: [
        {id: 1, name: "Jogador 1", idade: "X", timeid: "1", acoes:"?"  },
        {id: 2, name: "Jogador 2", idade: "X", timeid: "1", acoes:"?"  },
        {id: 3, name: "Jogador 3", idade: "X", timeid: "2", acoes:"?"  },
        {id: 4, name: "Jogador 4", idade: "X", timeid: "4", acoes:"?"  },
      ],
    };
  },
}
</script>
<template>
 <div class="container">
  <div class="title">
    <h2>Gerenciamento de jogadores</h2>
  </div>
  <div class="form-input">
    <input type="text" placeholder="Nome"> 
    <input type="text" placeholder="Time">
    <button>salvar</button>
  </div>
  {{ jogadores }}
  <div class="list-itens">
    <table>
      <thead>
        <tr>
          <th>ID</th>
          <th>Nome</th>
          <th>Idade</th>
          <th>Time ID</th>
          <th>Ações</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="jogador in jogadores" :key="jogador.id">
          <td>1</td>
          <td>Jogador 1</td>
          <td>X</td>
          <td>1</td>
          <td>???</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>
</template>
<style scoped>

</style>