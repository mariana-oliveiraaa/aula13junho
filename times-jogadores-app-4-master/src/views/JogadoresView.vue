<script>
export default {
  data() {
    return {
      jogadores: [
        { id: 1, name: "Joel", coluna_time_id: "Time 1", acao_id: "10 gols" },
        { id: 2, name: "João", coluna_time_id: "Time 2", acao_id: "10 gols" },
        { id: 3, name: "Mario", coluna_time_id: "Time 3", acao_id: "10 gols" },
        { id: 4, name: "Luiz", coluna_time_id: "Time 4", acao_id: "10 gols" },
      ],
    };
  },
};
</script>
<template>
  <div class="container">
    <div class="title">
      <h2>Gerenciamento de jogadores</h2>
    </div>
    <div class="form-input">
      <input type="text" placeholder="Nome" />
      <input type="text" placeholder="Time" />
      <button>Salvar</button>
    </div>
  </div>
  <div class="list-times">
    <table>
      <thead>
        <tr>
          <th>ID</th>
          <th>Nome</th>
          <th>Time ID</th>
          <th>Ações</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="jogador in jogadores" :key="jogador.id">
          <td>{{ jogador.id }}</td>
          <td>{{ jogador.name }}</td>
          <td>{{ jogador.coluna_time_id }}</td>
          <td>{{ jogador.acao_id }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>
