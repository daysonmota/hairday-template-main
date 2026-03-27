🧠 📅 O QUE O PROJETO FAZ <br>

👉 O HairDay é uma aplicação web de agendamento de horários. <br>

Funcionalidades: <br>
	•	📅 Selecionar uma data <br>
	•	⏰ Escolher horário disponível <br>
	•	👤 Informar nome do cliente <br>
	•	💾 Salvar agendamento (API fake com JSON Server) <br>
	•	📋 Listar agendamentos por dia <br>
	•	🗂️ Separar por período: <br>
	•	Manhã <br>
	•	Tarde <br>
	•	Noite <br>
	•	❌ Cancelar agendamento <br>


  <!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  
</head>
<body>

  <h1>💇 HairDay - Sistema de Agendamento</h1>

  <h2>📌 Descrição</h2>
  <p>
    Aplicação web para agendamento de cortes de cabelo.
    Permite criar, visualizar e organizar horários por período (manhã, tarde e noite).
  </p>

  <h2>⚙️ Tecnologias Utilizadas</h2>
  <ul>
    <li>JavaScript</li>
    <li>Webpack</li>
    <li>JSON Server (API fake)</li>
    <li>Babel</li>
    <li>Dayjs</li>
    <li>CSS</li>
  </ul>

  <h2>🚀 Configuração do Projeto</h2>

  <h3>1. Instalar JSON Server</h3>
  <pre>npm i json-server@1.0.0-alpha.21</pre>

  <h3>2. Criar .gitignore</h3>
  <pre>node_modules</pre>

  <h3>3. Configurar package.json</h3>
  <pre>
{
  "name": "hairday",
  "description": "Aplicação Web de agendamento para corte de cabelo",
  "author": "Dayson Rodrigues",
  "scripts": {
    "server": "json-server --watch server.json --port 3333",
    "build": "webpack",
    "dev": "webpack serve"
  }
}
  </pre>

  <h3>4. Criar arquivo server.json</h3>
  <pre>
{
  "schedules": []
}
  </pre>

  <h3>5. Rodar servidor</h3>
  <pre>npm run server</pre>

  <h3>6. Instalar Webpack</h3>
  <pre>npm i webpack webpack-cli --save-dev</pre>

  <h3>7. Criar arquivo de entrada</h3>
  <pre>src/main.js</pre>

  <h3>8. Criar webpack.config.js</h3>
  <p>Utilizar modelo padrão de configuração</p>

  <h3>9. Instalar Webpack Dev Server</h3>
  <pre>npm i webpack-dev-server --save-dev</pre>

  <h3>10. HTML Plugin</h3>
  <pre>npm i html-webpack-plugin --save-dev</pre>

  <h3>11. CSS Loader</h3>
  <pre>npm i style-loader css-loader --save-dev</pre>

  <h3>12. Importar CSS no main.js</h3>
  <pre>
"use strict"

import "./styles/global.css"
import "./styles/form.css"
import "./styles/schedule.css"
  </pre>

  <h3>13. Copiar Assets</h3>
  <pre>npm i copy-webpack-plugin --save-dev</pre>

  <h3>14. Babel</h3>
  <pre>
npm i babel-loader @babel/core @babel/preset-env --save-dev
  </pre>

  <h3>15. Executar projeto</h3>
  <pre>
npm run build
npm run server
npm run dev
  </pre>

  <h3>16. Instalar Dayjs</h3>
  <pre>npm i dayjs</pre>

  <h2>📂 Estrutura do Projeto</h2>
  <pre>
src/
 ├── main.js
 ├── styles/
 ├── services/
 │    ├── api-config.js
 │    ├── schedule-new.js
 │    ├── schedule-fetch-by-day.js
 ├── libs/
 └── assets/
  </pre>

  <h2>🔌 API (JSON Server)</h2>

  <h3>Base URL</h3>
  <pre>http://localhost:3333</pre>

  <h3>Rotas</h3>
  <ul>
    <li>GET /schedules → listar agendamentos</li>
    <li>POST /schedules → criar agendamento</li>
  </ul>

  <h2>🧠 Funcionalidades</h2>
  <ul>
    <li>Criar agendamento</li>
    <li>Filtrar por data</li>
    <li>Separar por período</li>
    <li>Cancelar agendamento</li>
  </ul>

</body>
</html>
