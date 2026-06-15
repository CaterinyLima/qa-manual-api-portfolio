# Caso de teste: CT-007 - Login com o campos usuario e senha vazios.

## Descrição
Garantir que o sistema impeça o login e exiba uma mensagem de alerta quando o formulário for submetido sem o preenchimendo dos campos "Username" e "Password".

---

## Informações Gerais

| Campo | Definição | 
| :--- | :--- |
| **Funcionalidades** | Login |
| **Tipo de teste** | Negativo |
| **Prioridade** | Alta |
| **Ambiente** | Staging | 

---

## Pré-condições
1. O navegador web deve estar aberto na página de login do sistema.

## Dados de Teste (Massa de dados)
* **Usuário:** [Vazio]
* **Senha:** [Vazio]

---

## Passos de Execução & Resultados

| Passo | Ação do Usuário | Resultado Esperado |
| :--- | :--- | :--- |
| **01** | Deixar o campo "Username" em branco. | O campo permanece vazio e sem a interação do sistema. |
| **02** | Deixar o campo "Password" em branco. | O campo permanece vazio e sem a interação do sistema. |
| **03** | Clicar no botão "Login". | O sistema barra o acesso e exibe a mensagem: `Epic sadface: Username is required`. |

---

## Pós-condições
* O utilizador permanece retido na tela de login (Acesso não autorizado).
* [Ver evidencia](./evidencias/CT-007-login-senha_e_usuario-vazios.png)