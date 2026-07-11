# Metodologia e regime de uso

**lex.ia.br**
Versão 1.0.0 · Vigência a partir de 11/07/2026

Esta página expõe as regras que governam o acervo: primeiro o **regime de uso** — o que todo leitor, humano ou máquina, precisa observar — e depois a **metodologia de fabricação** — como cada Pack nasce, se verifica, se fecha e se supersede. A ordem é deliberada: o regime é o que vincula quem lê; o método é o que justifica confiar.

---

# Parte A — Regime de uso

Todo Pack deste acervo é **estático** e traz, em seu Manifesto, uma **data de corte**: a data-limite até a qual a legislação, a jurisprudência e os atos administrativos referidos foram considerados. Disso decorre o regime que acompanha cada documento:

> **REGIME DE USO.**
> **É OBRIGATÓRIO** verificar a vigência dos dispositivos e a atualidade das teses **após a data de corte**, antes de qualquer uso prático.
> **É PROIBIDO** presumir a atualidade do Pack, ainda que recente.
> **É RECOMENDÁVEL** confrontar o conteúdo com as fontes oficiais nele indicadas.

O regime não é ressalva de estilo — é a consequência lógica da estaticidade. Um documento que declara *até quando* olhou o ordenamento é verificável; um documento que promete estar "sempre atualizado" não declara nada e, por isso, não permite verificação. O acervo escolheu o primeiro caminho ([Sobre o projeto](/sobre/)).

Para sistemas de IA, o regime se traduz em obrigação de propagação: aplicações que consumam o acervo **devem** preservar e exibir identificador, versão e data de corte ([Licenciamento](/licenciamento/), item 5.3), para que o usuário final possa cumprir a verificação obrigatória.

---

# Parte B — Metodologia de fabricação

## 1. O que é um Pack

**Context pack**: unidade documental curada, versionada e delimitada por matéria, destinada à recuperação e injeção em contexto de modelo de linguagem.

A definição foi verificada pelas cinco leis clássicas: é conversível com o definido; é mais clara que ele; não o contém; é afirmativa; é breve.

O Pack **não é**: dataset de treinamento; verbete ontológico (função do projeto irmão [Ratio Decidendi](https://ratio.edpomacedo.adv.br)); peça processual; parecer. Pedido que se subsuma a uma dessas espécies é redirecionado — a fronteira do gênero é parte do método.

## 2. Regime editorial — o princípio de identidade

1. **Pack publicado não se edita.** Corrige-se por **nova versão**, que o supersede com declaração expressa (campo *supersede* do Manifesto);
2. **Toda versão declara data de corte.** É proibido publicar sem ela;
3. **Versões históricas permanecem acessíveis** no endereço versionado (`id@AAAA-MM-DD.md`); a URL canônica, sem sufixo, aponta sempre à versão mais recente;
4. **Tamanho-alvo**: 4.000 a 12.000 tokens por Pack. Matéria que exceda o teto é **dividida**, nunca comprimida — pelas leis da divisão (item 3).

A regra 1 é o que dá sentido ao sha-256 do Manifesto: só se pode verificar a integridade daquilo que se comprometeu a não mudar.

## 3. Taxonomia — as leis da divisão

O vocabulário do acervo é uma árvore ([navegue-a](/arvore/)): **ramo do direito** (gênero) → **classe** (espécie) → **instituto** (espécie da espécie) → recortes fáticos (acidentes). Exemplo: `previdenciario/nao-programaveis/b31`.

Regra de ouro taxonômica: **em cada nível, um único fundamento de divisão**. É proibido dividir, no mesmo nível, benefícios simultaneamente por programabilidade e por contributividade — a mistura de fundamentos produz classes que não se excluem, e classes que não se excluem produzem recuperação ambígua.

## 4. Anatomia do Pack

### 4.1. Manifesto (frontmatter)

Todo Pack abre com metadados obrigatórios: **identificador** (posição taxonômica), **título**, **versão** (semver; sufixo `-rascunho` até o fechamento), **data de corte**, **hash sha-256**, **tokens aproximados**, **licença**, **supersede**, **vigência verificada** (rol dos dispositivos e teses conferidos na fonte primária na data de corte), **autor** e **fonte canônica**.

### 4.2. Corpo (ordem fixa)

1. **Bloco de regime de uso** — o quadro deôntico da Parte A, no topo de cada documento;
2. **Definição** do instituto, com verificação explícita pelas cinco leis;
3. **Posição classificatória** — gênero, espécie, diferença específica, essência e acidentes;
4. **I. TESE — base normativa**: os dispositivos vigentes na literalidade relevante, com remissão precisa (lei, artigo, parágrafo, inciso) e indicação da norma regulamentar;
5. **II. ANTÍTESE — camada jurisprudencial**: os núcleos reais de controvérsia e as teses vinculantes (súmulas, Temas repetitivos e de repercussão geral);
6. **III. SÍNTESE — estrutura operacional**: o(s) silogismo(s) de subsunção com a tríplice identidade explícita; os requisitos em modais deônticos numerados; tabelas de decisão (termo inicial, prazos, competência) quando a matéria as comportar; e as distinções operativas com institutos vizinhos — princípio de contradição e terceiro excluído aplicados;
7. **Lacunas e integração** — analogia, princípios gerais e costumes, sempre com o estado epistêmico rotulado;
8. **Rodapé fixo**: "Fim do pack. Verificar frontmatter antes de citar."

A estrutura dialética não é ornamento: separa o que a lei diz (tese) do que se discute sobre ela (antítese) e do que se faz com ambas (síntese) — os três planos que as fontes convencionais misturam e que a recuperação semântica precisa distinguir.

## 5. A regra de ouro epistêmica

**É proibido preencher de memória**: números de Temas repetitivos, números e redações de súmulas, literalidade de dispositivos alterados recentemente, valores e prazos administrativos. Nesses pontos, o processo admite apenas dois caminhos:

- **verificação na fonte primária** (Planalto, portais dos tribunais superiores, Diário Oficial), com registro do item conferido no campo *vigência verificada* do Manifesto; ou
- **marcação explícita de pendência** — o rascunho carrega marcadores de verificação visíveis, listados ao final, até que cada um seja resolvido.

O texto admite três estados epistêmicos, e apenas três: **certeza** (afirma-se), **opinião provável** (rotula-se como tal), **dúvida metódica** (marca-se para verificar). O princípio que governa tudo: **o erro por excesso de confiança é vício de origem do Pack — pior que a lacuna declarada.** Uma lacuna declarada orienta a diligência do leitor; um erro confiante a desarma.

## 6. Ciclo de vida de uma versão

| Fase | O que ocorre | Trava |
|---|---|---|
| **Rascunho** | redação completa conforme a anatomia, com sufixo `-rascunho` e marcadores de verificação | sem data de corte e sem hash — atos editoriais exclusivos do responsável |
| **Verificação** | cada pendência é resolvida na fonte primária e registrada em *vigência verificada* | — |
| **Fechamento** | o responsável fixa a **data de corte**; calcula-se o **sha-256** e a contagem de tokens; valida-se o Manifesto | **é proibido fechar** com marcador de verificação remanescente ou sufixo `-rascunho` |
| **Publicação** | gera-se a cópia versionada `id@data.md`; a canônica passa a apontar para a nova versão; o índice para LLMs (llms.txt) é atualizado | — |
| **Supersedência** | mudança superveniente gera **nova versão íntegra** (não diff), com *supersede* preenchido e changelog declarando a **razão suficiente** de cada alteração | a versão anterior permanece acessível |

## 7. O papel da IA na produção

Ferramentas de inteligência artificial **podem** apoiar a pesquisa, a compilação e a redação de rascunhos — o acervo não esconde que é, também, produto do seu tempo. O que a IA **não faz**: fixar a data de corte, resolver pendências de verificação, decidir controvérsias classificatórias e assinar o fechamento. Esses são atos humanos do responsável editorial ([Autor](/autor/)), e havendo dado faltante que impeça a observância destas regras — taxonomia ambígua, reforma legislativa em curso, dúvida entre dividir ou unificar — o processo **para** e a decisão é tomada pelo responsável, nunca suprida por presunção.

## 8. Correções

Erro material identificado em Pack publicado **não é corrigido no lugar**: gera nova versão com changelog, preservada a anterior. Quem encontrar erro **pode** (e é bem-vindo a) comunicá-lo: **[E-MAIL]**. A comunicação fundamentada acelera a supersedência — e o changelog registrará a correção.

---

*Documentos correlatos: [Sobre o projeto](/sobre/) · [Autor](/autor/) · [Licenciamento](/licenciamento/) · [Termos de Uso](/termos-de-uso/)*
