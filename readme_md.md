# ⚽ ArenaBet - Plataforma de Apostas Esportivas

**ArenaBet** é um sistema completo de gestão de apostas esportivas online desenvolvido em PHP e MySQL, oferecendo uma experiência moderna, fluida e segura tanto para os clientes quanto para os administradores.

---

## 🚀 Funcionalidades Principais

### 👤 Painel do Cliente (`/cliente/index.php`)
* **Gestão de Saldo e Apostas:** Visualização em tempo real do saldo disponível e atualização instantânea.
* **Depósito via PIX:** Sistema intuitivo com geração de dados de depósito e notificação ao administrador.
* **Solicitação de Saque PIX:** Aba dedicada para solicitação de resgate de fundos com validação de titularidade da conta bancária.
* **Gestão de Bilhetes:** Acompanhamento em tempo real dos palpites (Pendentes, Ganhos ou Perdidos).
* **Bloqueio de Apostas em Tempo Real:** Partidas que atingem o horário de início são trancadas automaticamente, marcadas com o selo **AO VIVO**.
* **Odds Especiais & Super Odds:** Suporte a cotações diferenciadas e mercados extras por partida.

---

### 🛡️ Painel Administrativo (`/admin/index.php`)
* **Autenticação Restrita:** Login de segurança para gestão do sistema.
* **Aprovação de Depósitos PIX:** Confirmação de pagamentos com liberação automática de saldo para a conta do usuário.
* **Gerenciamento de Saques:** Visualização de solicitações de saque com opções de **Aprovação** ou **Recusa com Estorno Automático** do saldo.
* **Cadastro de Jogos & Campeonatos:** Inclusão de partidas, odds para Casa/Empate/Fora, upload de escudos e adição de mercados extras (ex: autor do gol, cartões).
* **Encerramento de Partidas & Pagamentos:** Definição de placar real e apuração automática dos palpites vencedores com crédito imediato de prêmios aos clientes.

---

## 🛠️ Tecnologias Utilizadas

* **Backend:** PHP 8+ (PDO para conexões com banco de dados MySQL)
* **Frontend:** HTML5, CSS3, JavaScript (ES6)
* **Estilização:** [Tailwind CSS](https://tailwindcss.com/)
* **Ícones:** [Font Awesome 6](https://fontawesome.com/)
* **Banco de Dados:** MySQL 5.7+ / 8.0+

---

## 🗄️ Estrutura do Banco de Dados

O banco de dados `lean2352_apostasfutebol` é composto pelas seguintes tabelas principais:

* `usuarios`: Cadastro de clientes, e-mails, senhas criptografadas e saldo.
* `jogos`: Lista de partidas, escudos das equipes, odds principais, placar e status.
* `apostas`: Histórico de palpites dos usuários, odds fixadas e retornos calculados.
* `mercados_extras`: Odds adicionais por partida (ex: marcadores de gols).
* `depositos_pix`: Registro de avisos de depósito efetuados pelos clientes.
* `saques_pix`: Solicitações de resgate via PIX para análise administrativa.

---

## ⚙️ Como Instalar e Executar

1. Importe o arquivo SQL (`lean2352_apostasfutebol.sql`) para o seu servidor MySQL.
2. Configure as credenciais de acesso ao banco no arquivo `conexao.php`.
3. Certifique-se de que a pasta `uploads/escudos/` tenha permissões de escrita (`0755` ou `0777`).
4. Acesse o painel do cliente via `/cliente/index.php` e o painel admin via `/admin/index.php`.

---

© 2026 ArenaBet - Todos os direitos reservados.