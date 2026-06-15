# Caso de teste: CT-004 - Login com usuário invalido e senha correta.

## Descrição
Garantir que, ao preencher o campo usuario com a credencial inexistente e o campo de senha com dados válidos, o acesso seja negado, mantendo o usiário na tela de autenticação e exibindo uma mensagem de erro.

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
1. O nome do usuário a ser testado não deve constar na base de dados do sistema.
2. O navegador web deve estar aberto na página de login do sistema.

## Dados de teste (Massa de Dados)
* **Usuário** `standard`
* **Senha** `secret_sauce`

---

## Passos de execução & Resultado.

| Passo | Ação do usuário | Resultado Esperado |
| :--- | :--- | :--- |
| **01** | Introduzir o utilizador `standard` no campo "username". | O utilizador é inserido corretamente. | 
| **02** | Inserir a senha `secret_sauce` no campo "Password". | A senha é inserida e mascarada por segurança (ex:••••••••). |
| **03** | Clicar no botão "Login".| O sistema barra o acesso e exibe a mensagem: `Epic sadface: Username and password do not match any user in this service`.|

---

## Pós-condição
* O utilizador permanece retido na tela de login (Acesso nao autorizado).
* [Ver evidencia](./evidencias/CT-004-login-usuario-invalido.png)