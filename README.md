# desenvolvimento-web2
atividade de desenvolvimento web semana 2
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Formulário de Inscrição</title>

  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #eeeeee;
    }

    /* Caixa do formulário */
    .container-form {
      max-width: 500px;
      padding: 20px;
      margin: 20px auto;
      background-color: white;
    }

    /* Campos um embaixo do outro */
    form {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    /* Nome e e-mail lado a lado (bônus) */
    .linha {
      display: flex;
      justify-content: space-between;
    }

    .linha div {
      width: 48%;
    }

    label {
      font-size: 14px;
    }

    input, select {
      padding: 8px;
      border: 1px solid gray;
      border-radius: 5px;
      font-size: 16px;
    }

    /* Botão */
    button {
      background-color: #2c3e50;
      color: white;
      padding: 10px;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <div class="container-form">
    <h1>Inscreva-se</h1>

    <form method="get" action="">

      <div class="linha">
        <div>
          <label for="nome">Nome:</label>
          <input type="text" id="nome" name="nome" required minlength="3">
        </div>

        <div>
          <label for="email">E-mail:</label>
          <input type="email" id="email" name="email" required>
        </div>
      </div>

      <label for="idade">Idade:</label>
      <input type="number" id="idade" name="idade" required min="18" max="120">

      <label for="assunto">Assunto de interesse:</label>
      <select id="assunto" name="assunto" required>
        <option value="">Escolha...</option>
        <option value="html">HTML</option>
        <option value="css">CSS</option>
        <option value="javascript">JavaScript</option>
      </select>

      <label for="termos">
        <input type="checkbox" id="termos" name="termos" value="aceito" required>
        Aceito os termos
      </label>

      <button type="submit">Enviar</button>
    </form>
  </div>

</body>
</html>
