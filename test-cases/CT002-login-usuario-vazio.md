# 🧪 Caso de Teste: CT-002 - login-usuario-vazio

## 📝 Descrição
Garantir que o sistema impeça o login e exiba uma mensagem de alerta quando o formulário for submetido sem o preenchimento do campo "Username"
---

## ⚙️ Informações Gerais


| Campo | Definição |
| :--- | :--- |
| **Funcionalidade** | Autenticação de usuário / Login |
| **Tipo de Teste** | Negativo |
| **Prioridade** | Alta |
| **Ambiente** | Staging |

---

## 🔍 Pré-condições
1. O utilizador deve estar previamente registrado e com a conta ativa na base de dados.
2. O navegador web deve estar aberto na página de login do sistema.

## 📊 Dados de Teste (Massa de Dados)
* **Username:** [Vazio]
* **Password:** `secret_sauce`

---

## 🛠️ Passos de Execução & Resultados


| Passo | Ação do Usuário | Resultado Esperado |
| :---: | :--- | :--- |
| **01** | Deixar o campo "Username" em branco. | O campo permanece vazio e sem interações do sistema. |
| **02** | Inserir a senha `secret_sauce` no campo "Password". | A senha é inserida e mascarada por segurança (ex: ••••••••). |
| **03** | Clicar no botão "Login". | O sistema barra o acesso e exibe a mensagem: `Epic sadface: Username is required`. |

---

## 🏁 Pós-condições
* O utilizador permanece retido na tela de login (acesso não autorizado).
* (./evidencias/test-cases/CT-002-login-usuario-vazio.png)
