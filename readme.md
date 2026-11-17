# 🥤 FitFuel — Aplicativo de Pedidos para Academia

![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-A3E635?style=for-the-badge&labelColor=121214)
[![Ferramenta](https://img.shields.io/badge/Figma-Prot%C3%B3tipo_Interativo-38BDF8?style=for-the-badge&logo=figma&logoColor=white&labelColor=121214)](https://heap-pasta-46632846.figma.site/)
![Área](https://img.shields.io/badge/UI%2FUX_Design-Mobile_App-F4F4F5?style=for-the-badge&labelColor=121214)

Protótipo de alta fidelidade desenvolvido como desafio prático de **UI/UX Design**, abrangendo todas as etapas de concepção de produto digital: briefing, análise de usuário, Design System, wireframes, prototipagem lógica navegável e proposta de orçamento comercial.

🔗 **[ACESSAR PROTÓTIPO INTERATIVO NO FIGMA](https://heap-pasta-46632846.figma.site/)**

---

## 📋 1. Briefing e Análise do Projeto

* **Cliente / Nicho:** *PulseFit* — Rede de academias com lanchonete saudável interna e loja de suplementação.
* **Problema Identificado:** Nos horários de pico (18h às 21h), formam-se filas extensas no balcão da lanchonete, fazendo com que os alunos desistam de comprar shakes pós-treino ou refeições rápidas por falta de tempo.
* **Objetivo da Solução:** Criar um aplicativo de pedidos intuitivo que permita ao aluno solicitar shakes, marmitas fit e suplementos antes ou durante o treino, agendando a retirada expressa no balcão (sem filas) ou solicitando entrega via delivery.
* **Público-Alvo:** Alunos praticantes de atividades físicas (18 a 45 anos) que valorizam praticidade, agilidade no atendimento e transparência nutricional (calorias e macronutrientes).
* **Diferenciais Competitivos:**
  * Agendamento de preparo sincronizado com o tempo de treino;
  * Exibição clara de macronutrientes (proteínas, carboidratos e kcal) em cada item;
  * Retirada expressa via QR Code no balcão;
  * Função **"Pedir Novamente"** em 1 clique para itens de consumo diário.

---

## 🧠 2. UX Research (Persona e Jornada)

### Persona Principal
* **Nome:** Mariana Silva, 27 anos — Analista de Marketing.
* **Rotina:** Treina na hora do almoço ou logo após o expediente.
* **Dores:** Tem o tempo contado após o treino e detesta esperar na fila do balcão para pedir seu shake de Whey Protein.
* **Objetivos:** Fazer o pedido rapidamente pelo celular, controlar a ingestão diária de proteínas e retirar o produto pronto assim que sair do treino.

### Mapa da Jornada do Usuário
1. **Descoberta:** Abre o app antes de iniciar o treino e filtra pela categoria *Pós-Treino*.
2. **Personalização:** Escolhe o shake, seleciona o sabor e adiciona creatina extra.
3. **Configuração de Entrega:** Seleciona *Retirar no Balcão* e programa o preparo para daqui a 45 minutos.
4. **Pagamento:** Finaliza rapidamente via Pix Copia e Cola ou saldo de pontos.
5. **Retirada:** Recebe a notificação de *Pronto* ao terminar o treino e apresenta o QR Code no balcão sem pegar fila.

---

## 🎨 3. Design System & Style Guide

Para transmitir energia, modernidade e foco em performance esportiva, adotou-se uma interface **Dark Mode** de alto contraste.

### Paleta de Cores
| Token | Cor / Hex | Aplicação |
| :--- | :--- | :--- |
| **Background** | `#121214` | Fundo principal das telas |
| **Surface / Card** | `#202024` | Cartões de produtos, modais e inputs |
| **Primary (CTA)** | `#A3E635` | Botões principais, ícones ativos e destaques (texto em `#09090B`) |
| **Secondary** | `#38BDF8` | Badges nutricionais (ex: *"32g Proteína"*) e informações auxiliares |
| **Text Primary** | `#F4F4F5` | Títulos e textos principais |
| **Text Secondary** | `#A1A1AA` | Descrições, subtítulos e legendas |
| **Feedback** | `#22C55E` / `#EF4444` | Estados de sucesso e alertas de erro |

### Tipografia e Componentes
* **Família Tipográfica:** *Plus Jakarta Sans* / *Inter*
  * **H1 (Títulos de Tela):** 24px — Bold
  * **H2 (Seções):** 18px — SemiBold
  * **Body (Descrições):** 14px — Regular
  * **Caption (Tags e Macros):** 12px — Medium
* **Biblioteca de Componentes:** Botões (Primário, Secundário e Desabilitado), Chips de Categoria, Cards de Produto com badge nutricional, Seletor de Quantidade (`- 1 +`), Radio Buttons, Checkboxes e Tab Bar inferior.

---

## 📱 4. Wireframes e Prototipagem Lógica

O fluxo do aplicativo foi estruturado em **8 telas principais**, priorizando a zona de alcance do polegar (*Thumb Zone*) e a redução de carga cognitiva:

1. **Splash / Boas-Vindas:** Configurada com o *Flow Starting Point* principal do protótipo.
2. **Home / Cardápio:** Saudação personalizada, busca, filtros por objetivo (*Pré-treino, Pós-treino, Marmitas, Suplementos*) e destaques.
3. **Detalhes do Produto:** Tabela resumida de macros, seleção obrigatória de sabor e adicionais opcionais com atualização dinâmica de preço.
4. **Sacola / Carrinho:** Revisão de itens, aplicação de pontos de fidelidade e alternância entre **Retirada no Balcão** e **Delivery**.
5. **Checkout:** Escolha do horário de preparo (imediato ou agendado) e forma de pagamento.
6. **Acompanhamento de Status:** Linha do tempo em tempo real e geração de **QR Code** para retirada expressa.
7. **Histórico de Pedidos:** Listagem de pedidos anteriores com atalho *"Pedir Novamente"*.
8. **Perfil e Fidelidade:** Gestão de dados do aluno e carteira de pontos.

### Recursos Lógicos Aplicados no Figma
* **Variantes Interativas (*Interactive Components*):** Estados ativos/inativos nos seletores de sabor, adicionais e método de entrega.
* **Fluxo Condicional:** Caminhos distintos para *Retirada no Balcão* (taxa zero + agendamento de horário) e *Delivery* (cálculo de frete + endereço).
* **Microinterações e Overlays:** *Toast* de confirmação ao adicionar itens à sacola e transições suaves com *Smart Animate*.

### 📸 Capturas de Tela do Projeto

> *Substitua os caminhos abaixo pelas imagens salvas na pasta `/images` do seu repositório:*

| Design System | Wireframes | Telas de Alta Fidelidade |
| :---: | :---: | :---: |
| ![Design System](images/design-system.png) | ![Wireframes](images/wireframes.png) | ![Alta Fidelidade](images/alta-fidelidade.png) |

---

## 💰 5. Proposta de Orçamento Comercial

Simulação de orçamento profissional elaborado para apresentação ao cliente, considerando o escopo completo de UI/UX Design (valor/hora base de **R$ 75,00**):

| Etapa | Descrição dos Entregáveis | Horas Estimadas | Investimento (R$) |
| :--- | :--- | :---: | :---: |
| **1. Discovery & Briefing** | Imersão no negócio, definição de requisitos, Persona e Mapa de Jornada | 6h | R$ 450,00 |
| **2. Arquitetura & Wireframes** | Fluxograma lógico e criação de 8 telas em média fidelidade | 10h | R$ 750,00 |
| **3. Design System** | Paleta Dark Mode, tipografia, grid e biblioteca de componentes | 12h | R$ 900,00 |
| **4. UI Design & Protótipo** | Telas em alta fidelidade, variantes interativas e navegação completa | 16h | R$ 1.200,00 |
| **5. Handoff & Documentação** | Revisão de usabilidade, ajustes finais e organização para desenvolvimento | 6h | R$ 450,00 |
| **TOTAL** | **Prazo estimado de entrega: 3 semanas (15 dias úteis)** | **50h** | **R$ 3.750,00** |

### Condições Comerciais (Modelo)
* **Forma de Pagamento:** 40% na aprovação do briefing (R$ 1.500,00) e 60% na entrega final do protótipo navegável (R$ 2.250,00).
* **Incluso no Escopo:** Até 2 rodadas de revisão por etapa e acesso completo ao arquivo editável no Figma.
* **Não Incluso:** Desenvolvimento Front-end/Back-end e custos de publicação nas lojas de aplicativos.

---

## 👨‍💻 Autor

Desenvolvido por **[Seu Nome Completo]**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Conectar-0A66C2?style=flat&logo=linkedin&logoColor=white)](COLE_SEU_LINKEDIN)
[![GitHub](https://img.shields.io/badge/GitHub-Portf%C3%B3lio-181717?style=flat&logo=github&logoColor=white)](COLE_SEU_GITHUB)