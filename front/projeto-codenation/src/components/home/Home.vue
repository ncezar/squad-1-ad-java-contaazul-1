<template>
  <div>
    <label>Bem vindo {{usuario.nome}}.</label>
    <label>Seu token é {{usuario.token}}</label>
    <div class="margin">
      <select>
        <option value="producao">Produção</option>
        <option value="homologacao" selected>Homologação</option>
        <option value="Dev">Dev</option>
      </select>
      <select>
        <option value="ordenarPor">Ordenar Por</option>
        <option value="nivel" selected>Nivel</option>
        <option value="frequencia">Frequência</option>
      </select>
      <select>
        <option value="buscarPor">Buscar Por</option>
        <option value="nivel" selected>Nivel</option>
        <option value="descrição">Descrição</option>
        <option value="origem">Origem</option>
      </select>
      <input type="search" />
    </div>
    <div>
      <button class="arquivar">Arquivar</button>
      <button class="deletar">Apagar</button>
    </div>
    <div>
      <table>
        <thead>
          <tr>
            <th></th>
            <th>Nivel</th>
            <th>Log</th>
            <th>Eventos</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>
              <input type="checkbox" />
            </td>
            <td>das</td>
            <td>das</td>
            <td>das</td>
          </tr>
          <tr>
            <td>
              <input type="checkbox" />
            </td>
            <td>das</td>
            <td>das</td>
            <td>das</td>
          </tr>
          <tr>
            <td>
              <input type="checkbox" />
            </td>
            <td>das</td>
            <td>das</td>
            <td>das</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      usuario: {
        nome: "Larissa",
        token: "4d5748sdasd"
      }
    };
  }
};
</script>
<style scoped>
table {
  margin-top: 10px;
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width: 100%;
}
td,
th {
  border: 1px solid #dddddd;
  text-align: center;
  padding: 8px;
}
tr:nth-child(even) {
  background-color: #dddddd;
}
table,
th {
  border: 1px solid black;
}
button {
  border-radius: 4px;
  font-size: 15px;
  padding: 10px 20px;
  text-align: center;
  color: white;
  margin-top: 10px;
}
.arquivar {
  background-color: #4caf50;
}
.deletar {
  background-color: #f44336;
}
.margin {
  margin-top: 20px;
}
select {
  font-size: 15px;
  padding: 8px 15px;
  text-align: center;
  color: black;
}
input {
  font-size: 15px;
  padding: 8px 15px;
  text-align: left;
  color: black;
  width: 65%;
}
label {
  font-size: 20px;
  margin-top: 10px;
}
</style>