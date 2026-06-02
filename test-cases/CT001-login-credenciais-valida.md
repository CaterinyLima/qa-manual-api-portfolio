# 🧪 Caso de Teste: [CT-001] - [Login com credenciais válidas]

## 📝 Descrição
[Validar se o utilizador consegue autenticar-se com sucesso no sistema ao introduzir um nome de utilizador e uma palavra-passe válida, sendo direcionado para a página principal.]

---

## ⚙️ Informações Gerais

| Campo | Definição |
| :--- | :--- |
| **Funcionalidade** | [Autenticação de usuário / Login] |
| **Tipo de Teste** | [positivo] |
| **Prioridade** | [Alta] |
| **Ambiente** | [Staging / Homologação] |

---

## 🔍 Pré-condições
1. [O utilizador deve estar previamente registrado e com a conta ativa na base de dados.]
2. [O navegador web deve estar aberto na página de login do sistema.]

## 📊 Dados de Teste (Massa de Dados)
* **Usuário:** `standard_user`
* **Senha:** `secret_sauce`

---

## 🛠️ Passos de Execução & Resultados

| Passo | Ação do Usuário | Resultado Esperado |
| :---: | :--- | :--- |
| **01** | [Introduzir o utilizador `standard_user` no campo "Username".] | [O utilizador é inserido corretamente.] |
| **02** | [Inserir a senha `secret_sauce` no campo "Password".] | [A senha é inserida e mascarada por segurança (ex: ••••••••).] |
| **03** | [Clicar no botão "Login".] | [O sistema processa a operação, valida os dados e redireciona o utilizador para a página principal.] |

---

## 🏁 Pós-condições
* [O utilizador é autenticado com sucesso e mantido na sessão da página principal.]
* [Ver Evidência 01](./evidencias/test-cases/CT-001-Login-Sucesso-01.png)  
* [Ver Evidência 02](./evidencias/test-cases/CT-001-Login-Sucesso-02.png)