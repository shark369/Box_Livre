# 🚗 Box Livre

> Marketplace e plataforma inteligente de agendamento e intermediação de serviços automotivos para lava-jatos e centros de estética automotiva.

---

## 📌 Sobre o Projeto

O **Box Livre** conecta proprietários de veículos a estabelecimentos de limpeza e estética automotiva. A plataforma elimina atritos de espera física, permitindo que motoristas encontrem estabelecimentos próximos, comparem serviços e preços, visualizem a disponibilidade em tempo real e realizem agendamentos e pagamentos de forma 100% digital.

---

## 🎯 Proposta de Valor e Propósito

### ⚠️ Problemas Identificados
* **Espera imprevisível:** Longas filas e falta de precisão sobre o término do serviço quando o cliente deixa o veículo.
* **Barreiras de localização e comunicação:** Dificuldade do motorista (especialmente em novas cidades) de encontrar locais confiáveis, checar valores e saber se há vagas antes de se deslocar.
* **Gestão e ociosidade:** Dificuldade dos lava-jatos em organizar a lotação da agenda, gerenciar horários de pico e preencher horários ociosos.
* **Conflito de fluxo:** Risco de sobreposição entre atendimentos presenciais (*walk-in*) e agendamentos prévios.

### 💡 Nossa Solução
Um ecossistema centralizado com:
* Busca e filtragem por geolocalização e proximidade.
* Visualização da grade de disponibilidade e tempo estimado de espera por box.
* Reserva imediata sem conflitos e pagamento digital integrado.
* Painel de gerenciamento para lava-jatos otimizarem a capacidade e comunicação com clientes.

---

## 👥 Perfis de Acesso e Usuários

| Perfil | Atribuições |
| :--- | :--- |
| **🚗 Cliente / Motorista** | Busca estabelecimentos, compara serviços/preços, agenda horários em boxes livres, efetua pagamento digital e acompanha o status/tempo de término do serviço. |
| **🏢 Parceiro (Proprietário)** | Cadastra o estabelecimento, configura capacidade dos boxes, gerencia catálogo de serviços e define horários de funcionamento. |
| **🔧 Funcionário** | Gerencia os agendamentos operacionais no dia a dia, atualiza o status de atendimento e mantém comunicação com o cliente. |
| **🛡️ Administrador** | Gerencia cadastros de parceiros e clientes, moderação do sistema e métricas globais da plataforma. |

---

## 🏗️ Módulos e Componentes Arquiteturais

* **📅 Módulo de Agendamento & Disponibilidade:** Motor com controle rigoroso de concorrência para evitar *overbooking* e prevenir sobreposição de horários (atendimentos do app vs. presenciais).
* **🔍 Módulo de Catálogo & Busca:** Filtragem por proximidade, tipos de serviços (lavagem simples, completa, higienização, estética) e consulta de horários vagos.
* **💳 Módulo de Pagamentos:** Processamento financeiro integrado 100% digital.
* **⏱️ Módulo de Acompanhamento & Status:** Visualização do tempo de espera e status do serviço em tempo real.
* **🔔 Módulo de Notificações / Comunicação:** Alertas de confirmação, lembretes de agendamento e aviso de conclusão.
* **🔐 Módulo de Segurança & Autenticação:** Controle de acesso baseado em perfis (RBAC), sanitização de dados sensíveis e proteção de rotas.

---

## 💻 Stack Tecnológica

* **Front-end:** React (Aplicação Web)
* **Back-end:** Java com Spring Boot
* **Banco de Dados:** PostgreSQL (Relacional)
* **App Mobile:** *Não previsto inicialmente*

---

## ⚠️ Desafios Técnicos e Riscos Iniciais

* **Concorrência no Banco de Dados:** Garantir consistência transacional e bloqueio otimista/pessimista na reserva simultânea de boxes.
* **Sobreposição de Horários:** Sincronização entre a fila presencial física do lava-jato e os agendamentos remotos via app.
* **Disponibilidade e Carga:** Dimensionamento de infraestrutura e hospedagem para suportar picos de acesso.

---

## 👥 Equipe do Projeto

| Nome | Papel |
| :--- | :--- |
| **Emanuel Diogo** | Product Owner & DevOps |
| **Luiz Filipe** | Scrum Master |
| **Samuel Alves** | QA |
