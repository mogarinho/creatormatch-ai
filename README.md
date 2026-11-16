# creatormatch-ai
Protótipo e artigo técnico sobre matchmaking entre e-commerce e criadores usando LLMs e regras determinísticas.
# CreatorMatch AI — Conexão Inteligente entre E-commerce e Criadores com LLMs

> **Projeto Hands-On & Artigo Técnico Aplicado**  
> Desenvolvido para o Bootcamp **Bradesco — Agentes de IA: do Zero à Prática** na [DIO](https://dio.me).

---

## 📌 Visão Geral do Projeto

O **CreatorMatch AI** é um sistema inteligente que conecta lojas de e-commerce e varejo (com foco em lojas de variedades) a micro e médios criadores de conteúdo relevantes.

O projeto resolve o problema da **miopia das métricas de vaidade** (contratar apenas por número bruto de seguidores) através de uma **arquitetura híbrida**:
1. **Gate Eliminatório de Segurança:** Barra perfis com risco reputacional ou desalinhamento demográfico gritante sem gastar tokens.
2. **Matriz Determinística de 100 Pontos:** Avaliação objetiva inspirada em auditorias profissionais de agências (Afinidade, Demografia, Engajamento, Produção, Conversão e Viabilidade).
3. **Pacote de Campanha em 4 Módulos:** Gera Outreach, *Do's & Don'ts*, Menu Criativo com 3 opções de roteiro (Trend Viral + 2 formatos nativos do criador) e governança com UTMs e KPIs de funil.

---

## 🖥️ Demonstração Visual do Protótipo

A interface do protótipo foi modelada com base em referências do **Dribbble** e prototipada para validar o fluxo operacional:

* **Dashboard Principal:** Tabela de ranqueamento dos criadores com scores coloridos, status de recomendação e filtros por produto.
* **Modal Interativo de Campanha:** Exibição do breakdown da pontuação, abordagem comercial, roteiros e métricas de desempenho.

*(Para rodar o protótipo localmente, basta abrir o arquivo `dashboard_creatormatch.html` em qualquer navegador).*

---

## 🧪 O Experimento Prático (Resultados com Dados Reais)

Testamos o produto **Gloss Labial Efeito Volume (R$ 29,90)** contra criadores e arquétipos de audiência reais:

| Criador (Referência Real) | Nicho Editorial | Base Estimada | Status no Gate | Score (100 pts) | Veredito Estratégico |
|---|---|---|:---:|:---:|---|
| **Joyce Kitamura** | Beleza & Skincare | ~600k Instagram | **Aprovada** | **95 / 100** | **Recomendada (Autoridade Técnica)** |
| **Camila Pudim** | Trends & Makes Virais | ~4.5M Instagram | **Aprovada** | **88 / 100** | **Recomendada (Volume & Viralização)** |
| **Amanda Looks** | Achadinhos & Moda | 27k Instagram | **Aprovada** | **87 / 100** | **Recomendada (Match Comercial)** |
| **Nath Finanças** | Educação Financeira | ~550k Instagram | **REPROVADA** | — | **Descarte por Risco Editorial / Combate a Compras Supérfluas** |
| **Casimiro Miguel (Cazé)** | Futebol & Games | >4M Instagram | **REPROVADA** | — | **Descarte por Incompatibilidade Demográfica (>75% M)** |

---

## 📦 Estrutura do Pacote de Campanha (Exemplo Joyce Kitamura)

1. **Abordagem (Outreach):** Mensagem inicial personalizada e respeitosa para Direct/E-mail de assessoria.
2. **Compliance (Do's & Don'ts):** Exigência de `#publi`, proibição de alegações falsas de procedimento estético definitivo.
3. **Menu Criativo Colaborativo:**
   - *Opção 1 (Trend Viral):* Lip combo acessível de gringa por menos de R$ 30.
   - *Opção 2 (Nativo Técnico):* Resenha sincera de textura e aplicador.
   - *Opção 3 (Contextual):* Inserção em make rápida de 5 minutos do dia a dia.
4. **Setup de Performance:**
   - Link UTM parametrizado: `mixvariedades.com.br/gloss-volume?utm_source=instagram&...`
   - Cupom exclusivo: `JOYCE10` (10% OFF)
   - Metas de Funil: Retenção 3s $>55\%$, CTR $>2.5\%$, Conversão $>1.8\%$ e ROAS $>2.5\times$.

---

## 📂 Arquivos Deste Repositório

- `ARTIGO.md`: Artigo técnico completo e aprofundado, pronto para leitura e publicação na comunidade DIO.
- `dashboard_creatormatch.html`: Protótipo interativo completo (HTML5 + Tailwind CSS + FontAwesome).

---

## 🚀 Como Executar o Projeto

1. Clone o repositório ou baixe os arquivos.
2. Dê dois cliques em `dashboard_creatormatch.html` para abrir o protótipo navegável no navegador.
3. Leia o artigo completo em `ARTIGO.md` para entender as decisões de arquitetura e engenharia de prompt.

---
*Desenvolvido como entrega prática no Bootcamp Bradesco — Agentes de IA da Digital Innovation One.*
