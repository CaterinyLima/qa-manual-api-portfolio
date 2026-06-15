# Caso de teste: CT-006 - Login com usuário e senha incorretos.

## Descrição
Garantir que ao preencher o campo uruário e o campo senha com as credenciais inválidas, o acesso seja negado, mantendo o usuário na tela de autenticação e exibindo uma mensagem de erro.

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
1. o navegador web deve estar aberto na página de login do sistema.

## Dados de teste (Massa de Dados)
* **Usuário** `standard`
* **Senha** `secretsauce_`

---

## Passo de Execução & Resultado.

| Passo | Ação do Usuário | Resultado Esperado | 
| :--- | :--- | :--- |
| **01** | Introduzir o utilizador `standard` no campo "username". | O utilizador é inserido corretamente. |
| **02** | Inserir a senha `secretsauce_` no campo "Password". | A senha é inserida e mascarada por segurança (ex:••••••••). |
| **03** | Clicar no botão "Login". | O sistema barra o acesso e exibe a mensagem: `Epic sadface: Username and password do not match any user in this service`.|

---

## Pós-condição
* O utilizador permanece retido na tela de login (Acesso não autorizado).
* [ver evidencia](./evidencias/CT-006-login-senha_e_usuario-invalidos.png)