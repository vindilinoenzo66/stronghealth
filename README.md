<div align="center">

# 💪 Strong Health
### Academia Digital de Suplementação

*E-commerce especializado em suplementos alimentares para praticantes de musculação, atletas e entusiastas de vida saudável.*

![Status](https://img.shields.io/badge/status-em%20desenvolvimento-2ECC71?style=flat-square)
![Versão](https://img.shields.io/badge/versão-1.0-26293A?style=flat-square)
![Ano](https://img.shields.io/badge/ano-2026-7B56D3?style=flat-square)
![Licença](https://img.shields.io/badge/licença-MIT-F5C443?style=flat-square)

</div>

---

## 📋 Sobre o Projeto

O **Strong Health** é uma plataforma de e-commerce voltada à venda de suplementos alimentares, desenvolvida como projeto acadêmico da disciplina de **Projeto de Interface de Usuário**. A proposta central é oferecer uma experiência de compra intuitiva, segura e completa — da descoberta do produto até o rastreamento do pedido —, guiada pela metáfora de uma **academia digital**.

Assim como em uma academia física, o usuário encontra os "equipamentos" certos (produtos), recebe orientação de um "personal trainer digital" (filtros e blog), monta sua "ficha de treino" (carrinho), finaliza o treino (pagamento) e acompanha sua evolução (rastreamento de pedidos). Toda a operação é gerenciada pela "administração da academia" (painel administrativo).

---

## ✨ Funcionalidades

### Para o Cliente
- **Catálogo de produtos** com filtros por categoria, marca, objetivo (hipertrofia, emagrecimento, performance) e faixa de preço
- **Cadastro e login** com recuperação de senha por e-mail
- **Carrinho de compras** persistente entre sessões
- **Checkout completo** com suporte a Cartão de Crédito (até 12x), Débito, Pix e Boleto bancário
- **Rastreamento de pedidos** com status em tempo real
- **Avaliações de produtos** com nota de 1 a 5 estrelas e comentário
- **Blog** com artigos especializados em nutrição e performance

### Para o Administrador
- **Painel administrativo** centralizado
- Gestão de produtos, categorias e estoque com alertas de baixo estoque
- Processamento e atualização de status de pedidos
- Moderação de avaliações dos clientes
- Publicação e gerenciamento de artigos no blog
- Relatórios de vendas (totais por período, produtos mais vendidos, clientes recorrentes)

---

## 🎨 Design System

### Metáfora
> **"Academia Digital de Suplementação"** — o usuário entra para encontrar os equipamentos certos para alcançar seus objetivos de saúde, treino e performance.

| Elemento da Academia | Representação na Interface |
|---|---|
| Entrada da academia | Página inicial com destaques e promoções |
| Equipamentos de treino | Produtos do catálogo |
| Personal trainer | Filtros, recomendações e blog |
| Ficha de treino | Carrinho de compras |
| Avaliação física | Avaliações e comentários dos produtos |
| Recepção / caixa | Pagamento online |
| Acompanhamento de evolução | Rastreamento de pedidos |
| Administração da academia | Painel administrativo |

### Paleta de Cores

| Cor | Hex | Uso |
|---|---|---|
| 🟢 Verde Saúde | `#2ECC71` | Botões principais, ações positivas, identidade da marca |
| 🟡 Amarelo Energia | `#F5C443` | Promoções, destaques e selos |
| 🟣 Roxo Performance | `#7B56D3` | Banners e títulos secundários |
| 🔵 Azul-Claro Equilíbrio | `#66CCFF` | Áreas informativas e elementos de confiança |
| ⬛ Grafite Neutro | `#26293A` | Textos principais, cabeçalhos e rodapé |
| ⬜ Branco Neutro | `#FFFFFF` | Fundo de cards e áreas de leitura |

### Tipografia

Família: **Barlow** (Google Fonts) — sans-serif moderna inspirada em sinalização de rodovias, transmitindo força, clareza e performance.

| Peso | Uso |
|---|---|
| ExtraBold 800 | Logotipo, hero/banner principal e headlines de campanha |
| Bold 700 | Nomes de produtos, títulos de seção e menu de navegação |
| SemiBold 600 | Botões (CTAs), subtítulos de cards e filtros |
| Regular 400 | Descrições de produtos, corpo do blog e formulários |
| Condensed Bold | Selos de desconto, badges promocionais e tags de estoque |
| Light 300 | Rodapé, disclaimers e textos auxiliares |

### Ícones

Biblioteca **Font Awesome** (`react-icons/fa`), formato SVG escalável, cor primária Verde Saúde `#2ECC71`.

Ícones utilizados: carrinho, busca, avaliação por estrelas, entrega/caminhão, cartão de crédito, caixa de produto, blog, folha (natural), raio (pré-treino) e escudo (segurança).

---

## 🗂 Requisitos de Software

### Requisitos Funcionais

| ID | Funcionalidade |
|---|---|
| RF01 | Cadastro de clientes (nome, e-mail único, senha, CPF, data de nascimento, endereço) |
| RF02 | Autenticação com login/senha e recuperação por e-mail; sessões expiram em 30 min |
| RF03 | Catálogo com foto, nome, descrição, preço, marca, categoria, avaliação média e filtros |
| RF04 | Carrinho de compras com persistência entre sessões |
| RF05 | Pagamento via Cartão (até 12x), Débito, Pix e Boleto com atualização por webhook |
| RF06 | Controle de estoque automático com alertas de limite mínimo configurável |
| RF07 | Avaliações de produtos (1–5 estrelas) com moderação antes da publicação |
| RF08 | Blog com artigos indexáveis por mecanismos de busca |
| RF09 | Painel administrativo com gestão de produtos, pedidos, estoque, blog e relatórios |

### Requisitos Não Funcionais
- Interface responsiva para dispositivos móveis e desktop
- Processamento de pagamentos em conformidade com **PCI-DSS**
- Disponibilidade mínima de 99,5%
- Tempo de resposta inferior a 2 segundos para operações principais

---

## 👥 Equipe

| Nome | Papel |
|---|---|
| **Rick Li** | Front-end / UI Design |
| **Enzo Vindilino** | Back-end / Banco de Dados |
| **Cayke Chen** | UX / Prototipação |
| **Matheus Ubinha** | Design System / Tipografia |

---

## 📁 Estrutura do Repositório

```
strong-health/
├── docs/
│   ├── SRS_Loja_Suplementacao.docx   # Especificação de Requisitos
│   ├── BAD_Banco_de_Dados.pdf        # Normalização do Banco de Dados
│   ├── tipografia.pdf                # Proposta tipográfica
│   └── metafora-cores.pdf            # Metáfora e esquema de cores
├── design/
│   └── enzoid.html                   # Design system / protótipo HTML
├── apresentacao/
│   └── LojaSuplementacao_Apresentacao.pptx
└── README.md
```

---

## 🏫 Contexto Acadêmico

> Projeto desenvolvido para a disciplina de **Projeto de Interface de Usuário** — 2026.
> Instituição de Ensino Superior — Turma de Análise e Desenvolvimento de Sistemas.

---

<div align="center">
  <sub>© 2026 Strong Health · Rick Li · Enzo Vindilino · Cayke Chen · Matheus Ubinha</sub>
</div>
