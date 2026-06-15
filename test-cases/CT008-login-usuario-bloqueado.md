# Caso de Teste: CT-008 - Login com usuario bloqueado.

## Descrição
Garantir que o sistema inpeça o login e exiba uma mensagem de alerta quando o formulário for submetido com o preenchimento de um usuário bloqueado.

---

## Informações Gerais 

| Campo | Definiçao |
| :--- | :--- |
| **Funcionalidade:** | Login | 
| **Tipo de Teste** | Negativo | 
| **Prioridade** | Alta |
| **Ambiente** | Staging |

---

## Pré-condições
1. O ultilizador deve estar previamente registrado e com a conta bloqueada na base de dados.
2. O navegador web deve estar aberto na página de login do sistema.

## Dados do Teste (Massa de Dados)
* **Usuário:** `locked_out_user`
* **Senha:** `secret_sauce`

---

## Passos de Execução & Resultados

| Passo | Ação do Usuádio | Resultado Esperado | 
| :--- | :--- | :--- |
| **01** | Introduzir o utilizador `locked_out_user` no campo "Username". | O utilizador é inserido corretamente. |
| **02** | Inserir a senha `secret_sauce` no campo "Password". | A senha é inserida e mascarada por segurança (ex: ••••••••). |
| **03** | Clicar no botão "Login". | O sistema barra o acesso e exibe a mensagem: `Epic sadface: Sorry, this user has been locked out`. |

---

## Pós-condição
* O utilizador permanece retido na tela de login (Acesso não autorizado).
* [Ver evidência](./evidencias/CT-008-login-usuario-bloqueado.png)