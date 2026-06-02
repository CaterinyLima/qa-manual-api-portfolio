# Caso de teste: CT-003 - login campo senha vazio

## Descrição
Garantir que o sistema impeça o login e exiba uma mensagem de alerta quando o formulário for submetido sem o preenchimento do campo "Password"

---

## Informações Gerais

| Campo | Definição |
| :--- | :--- |
| **Funcionalidade** | Login |
| **Tipo de teste** | Negativo |
| **Prioridade** | Alta |
| **Ambiente** | Staging |

---

## Pré-condições 
1. O utilizador deve estar previamente registrado e com conta ativa na base de dados.
2. O navegador web deve estar aberto na página de login do sitema.

## Dados de teste (Massa de Dados)
* **Usuário:** `locked_out_user`
* **Senha:** [Vazio]

---

## Passos de Execução & Resultados

| Passo | Ação do usuário | Resultado Esperado |
| :--- | :--- | :---|
| **01** | Introduzir o utilizador `locked_out_user` no campo "Username". | O utiliazador é inserido corretamente. |
| **02** | Deixar o campo "*Password" em branco. | O campo permanece vazio e sem interações do sistema. | 
| **03** | Clicar no botão "Login" | O sistema barra o acesso e exibe a mensagem: `Epic sadface: Password is required`.

---

## Pós-condições
* O utilizador permanece retido na tela de login (Acesso não autorizado).
* [Ver Evidência](./evidencias/test-cases/CT-003-login-senha-vazio.png)