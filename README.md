[ux_ui_case_study_aura_beauty.md](https://github.com/user-attachments/files/33939996/ux_ui_case_study_aura_beauty.md)
# 💄 Case Study UX/UI: Otimização de Conversão para E-Commerce de Beleza

> **Como um Redesign Orientado à Psicologia de UX e Diversidade Pode Elevar a Taxa de Conversão em E-Commerce**

![UX UI Before and After Comparison](https://raw.githubusercontent.com/placeholder/aura-beauty-case/main/assets/before-after-cover.png)

---

## 📌 Sumário
- [Visão Geral do Projeto](#-visão-geral-do-projeto)
- [O Desafio](#-o-desafio)
- [Diagnóstico da Interface Anterior (Antes)](#-diagnóstico-da-interface-anterior-antes)
- [Soluções de Design & UX (Depois)](#-soluções-de-design--ux-depois)
- [Princípios de Ciência Comportamental Aplicados](#-princípios-de-ciência-comportamental-aplicados)
- [Design System & Especificações Técnicas](#-design-system--especificações-técnicas)
- [Estrutura de Protótipo e Interatividade (Figma)](#-estrutura-de-protótipo-e-interatividade-figma)
- [Métricas Impactadas (Resultados Esperados)](#-métricas-impactadas-resultados-esperados)

---

## 🔍 Visão Geral do Projeto

Este estudo de caso analisa a otimização da **Página de Detalhes do Produto (PDP)** da marca fictícia **Aura Beauty** (item: *Aura Velvet Lipstick*). 

O objetivo principal foi transformar uma interface genérica e estática em uma experiência imersiva, inclusiva e focada na redução de atrito de conversão (CRO), aproveitando gatilhos visuais e psicológicos específicos do segmento de cosméticos.

---

## 🎯 O Desafio

No segmento de maquiagem e cuidados pessoais, a compra online enfrenta uma grande barreira: **o consumidor não pode testar o produto fisicamente**. 

A interface original falhava em responder às dúvidas críticas do usuário no momento da decisão:
1. *"Como esse tom de batom vai ficar no meu tom de pele?"*
2. *"A textura é confortável ou resseca os lábios?"*
3. *"Vale a pena assinar para receber periodicamente ou comprar avulso?"*

---

## ❌ Diagnóstico da Interface Anterior (Antes)

| Elemento | Falha de UX/UI | Impacto Negativo |
| :--- | :--- | :--- |
| **Imagem Principal** | Produto isolado em base neutra sem aplicação humana. | **Imagination Gap:** O usuário não consegue visualizar a cor real na pele. |
| **Prova Social** | Número redondo genérico (`200+ Reviews`). | Falta de autenticidade; gera desconfiança sobre a veracidade das avaliações. |
| **Seletor de Cor** | Menu suspenso (*Dropdown*) apenas com texto (`Ruby Red`). | Exige cliques extras e oculta as opções de cores disponíveis. |
| **Planos de Compra** | Botões de rádio empilhados com o mesmo peso visual. | Leva o usuário a escolher a opção de menor valor por padrão (compra única). |
| **Chamada para Ação (CTA)** | Texto transacional básico (`ADD TO CART`). | Remete apenas ao ato de gastar dinheiro. |
| **Selos de Confiança** | Lista de texto sem destaque visual ou relevância para o nicho. | Baixa retenção visual e pouca quebra de objeções. |

---

## ✨ Soluções de Design & UX (Depois)

### 1. Fim da "Lacuna de Imaginação" (*Imagination Gap*)
* **Substituição da imagem fria** por um painel dinâmico que exibe o batom aplicado em **diferentes tons de pele** (clara, morena, negra) e amostras reais de textura (*swatches*).
* **Benefício:** Reduz o esforço cognitivo e permite autoidentificação imediata.

### 2. Efeito Halo & Prova Social de Alta Precisão
* **Adição do Badge de Destaque:** `★ MAIS VENDIDO` posicionado no topo para ancoragem de valor.
* **Métricas Precisas:** Atualização para `4.9 ★ (221 avaliações)` acompanhado de prova social em tempo real (`🔥 512 vendidos esta semana`).

### 3. Seleção Visual Dinâmica (Swatches + Tooltip)
* **Amostras Circulares de Cor:** Substituição do dropdown por botões visuais que mostram a cor exata.
* **Microinteração:** *Tooltip* ao passar o cursor com a descrição do acabamento e sensação (*"Ruby Red • Vermelho clássico de tom frio, matte aveludado e confortável"*).

### 4. Cards Lado a Lado & Destaque de Recorrência (AOV)
* **Arquitetura de Escolha:** Apresentação da *Assinatura Aura Club* em um card de destaque com tag `MAIS VANTAGEM`, destacando o desconto de 15% e benefícios como cancelamento simples e frete grátis.

### 5. CTA Emocional e Ícones de Nicho
* **Botão Orientado ao Benefício:** `GARANTIR MEU TOM ✨` em vez de termos genéricos.
* **Garantias Ilustradas:** Substituição de textos genéricos por ícones relevantes: `100% Vegano & Cruelty-Free`, `Testado Dermatologicamente` e `30 Dias de Garantia`.

---

## 🧠 Princípios de Ciência Comportamental Aplicados

```
┌─────────────────────────────────────────────────────────────────┐
│                      PSICOLOGIA DO CONSUMIDOR                   │
├──────────────────────────┬──────────────────────────────────────┤
│ Princípio                │ Aplicação Prática na Interface       │
├──────────────────────────┼──────────────────────────────────────┤
│ 1. Efeito Halo           │ Badge "Mais Vendido" e Nota 4.9     │
│ 2. Prova Social Específica│ "512 vendidos esta semana"           │
│ 3. Revelação Progressiva │ Tooltip descritivo em cada swatch    │
│ 4. Ancoragem de Preço    │ Destaque do plano recorrente        │
│ 5. Redução de Objeções   │ Selos cruelty-free e dermatológicos │
└──────────────────────────┴──────────────────────────────────────┘
```

---

## 🎨 Design System & Especificações Técnicas

### Palette de Cores
```css
:root {
  /* Surfaces */
  --bg-primary: #FAF8F5;
  --bg-card-featured: #F4EFE6;
  
  /* Text & Actions */
  --text-primary: #1A1A1A;
  --text-secondary: #666666;
  --btn-primary: #2B1D1D;
  
  /* Accents */
  --accent-gold: #8C743E;
  --accent-fire: #C8521A;
  
  /* Product Swatches */
  --swatch-ruby: #B81D24;
  --swatch-berry: #8A1C3B;
  --swatch-plum: #753448;
  --swatch-mauve: #B65163;
  --swatch-classic: #D12028;
}
```

### Tipografia
* **Headings:** `Playfair Display` (SemiBold / 32px)
* **Body / Labels:** `Inter` ou `Plus Jakarta Sans`
  * *Body Regular:* 14px / Line-height: 1.5
  * *CTA / Buttons:* 15px / Bold / Letter-spacing: +0.5px
  * *Badges:* 11px / Bold / Uppercase

---

## 🛠️ Estrutura de Protótipo e Interatividade (Figma)

Para recriar este projeto no Figma com navegação interativa:

1. **Variantes de Componente:**
   * Crie o componente `Swatch` com os estados `Default` e `Selected`.
   * Crie as variantes da `Galeria Hero` trocando a imagem principal conforme a cor selecionada.
2. **Conexão de Protótipo:**
   * `On Click` no swatch de cor -> `Change to` -> variante correspondente na galeria.
   * `On Hover` no swatch -> Exibir frame overlay do `Tooltip`.

---

## 📈 Métricas Impactadas (Resultados Esperados)

* **+28% na Taxa de Conversão (CVR):** Impulsionada pela redução da indecisão de cor e inclusão visual.
* **+18% no Ticket Médio (AOV):** Através do destaque visual do plano de assinatura e pacotes.
* **-35% na Taxa de Rejeição (Bounce Rate):** Com informações claras e quebra imediata de objeções éticas e de dermatologia.

---

## 👤 Autor

Desenvolvido como estudo de caso de UX/UI & CRO para e-commerce.

- **LinkedIn:** [Seu Nome / Link do Perfil]
- **Figma:** [Link para o Arquivo Comunitário]

---
*Se este projeto ajudou nos seus estudos, não se esqueça de deixar uma ⭐️ neste repositório!*
