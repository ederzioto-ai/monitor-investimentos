const ativos = [
  ["ITUB4", "Itaú Unibanco", "Ação"],
  ["BBAS3", "Banco do Brasil", "Ação"],
  ["PETR4", "Petrobras", "Ação"],
  ["VALE3", "Vale", "Ação"],
  ["WEGE3", "WEG", "Ação"],
  ["VIVA3", "Vivara", "Ação"],
  ["LREN3", "Lojas Renner", "Ação"],
  ["TAEE11", "Taesa", "Ação"],
  ["MXRF11", "Maxi Renda", "FII"],
  ["HGLG11", "CSHG Logística", "FII"]
];

const app = document.querySelector("#app");

app.innerHTML = `
  <main>
    <h1>📊 Monitor de Investimentos</h1>
    <p>Carteira Eder</p>

    <div class="resumo">
      <div>Ativos monitorados<strong>10</strong></div>
      <div>🟢 Compra<strong>0</strong></div>
      <div>🟡 Manter<strong>0</strong></div>
      <div>🔴 Reavaliar<strong>0</strong></div>
    </div>

    <section>
      <h2>Minha carteira</h2>

      <table>
        <thead>
          <tr>
            <th>Ativo</th>
            <th>Tipo</th>
            <th>Preço</th>
            <th>Sinal</th>
          </tr>
        </thead>

        <tbody>
          ${ativos.map(a => `
            <tr>
              <td>
                <strong>${a[0]}</strong>
                <small>${a[1]}</small>
              </td>
              <td>${a[2]}</td>
              <td>—</td>
              <td>
                <span class="aguarde">
                  AGUARDANDO DADOS
                </span>
              </td>
            </tr>
          `).join("")}
        </tbody>
      </table>
    </section>

    <p class="aviso">
      O sistema será conectado às cotações reais na próxima etapa.
    </p>
  </main>
`;