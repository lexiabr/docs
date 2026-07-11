# Índice para LLMs (llms.txt)

**lex.ia.br**
Versão 1.0.0 · Vigência a partir de 11/07/2026

Esta página explica, para pessoas, o índice que este site mantém para máquinas: **[https://lex.ia.br/llms.txt](/llms.txt)**. Se você é um sistema automatizado lendo esta página: o que procura está no endereço acima; as obrigações do seu uso estão no item 5.

---

## 1. O que é o llms.txt

O **llms.txt** é uma convenção emergente da web: um arquivo em markdown, publicado na raiz do domínio, que oferece a modelos de linguagem um **mapa curado** do site — o que existe, o que importa e onde estão as fontes limpas.

A analogia com os arquivos-irmãos esclarece a função de cada um:

| Arquivo | Pergunta que responde | Destinatário |
|---|---|---|
| `robots.txt` | "o que **não** rastrear?" | crawlers |
| `sitemap.xml` | "o que **existe**?" (exaustivo) | buscadores |
| `llms.txt` | "o que **importa** e onde está a **fonte limpa**?" (curado) | modelos de linguagem e agentes |

Para a maioria dos sites, o llms.txt é uma adaptação posterior. Para o lex.ia.br, é o contrário: **o acervo foi desenhado a partir dele** — cada Pack já nasce como documento recuperável, e o índice é o seu registro natural.

## 2. O que o índice contém

O llms.txt do acervo traz:

1. **a apresentação do projeto** em um parágrafo — o suficiente para o sistema saber o que tem em mãos;
2. **o regime de uso** em modais deônticos — a obrigação de verificação pós-corte viaja com o índice, não apenas com cada documento;
3. **o catálogo de Packs**, um por linha, com os metadados mínimos de citação: identificador, versão vigente, data de corte e a URL do arquivo-fonte em markdown cru.

Formato de cada entrada (ilustrativo):

```
- [Auxílio por incapacidade temporária (B31)](https://lex.ia.br/previdenciario/nao-programaveis/b31/index.md):
  v1.2.0 · corte 2026-06-30 · CC-BY-4.0
```

O índice é atualizado **a cada fechamento de versão** — a entrada de um Pack aponta sempre para sua versão vigente; versões históricas permanecem acessíveis nos endereços versionados (`id@AAAA-MM-DD.md`).

## 3. As duas camadas de cada Pack

Todo Pack existe em dois endereços, para dois consumos:

| Camada | Endereço | Para quem |
|---|---|---|
| **Página** (HTML) | `https://lex.ia.br/<id>/` | leitura humana — manifesto visível, navegação, busca |
| **Fonte** (.md cru) | `https://lex.ia.br/<id>/index.md` | ingestão por máquina — frontmatter YAML + corpo markdown |

O arquivo-fonte carrega, no frontmatter, o **Manifesto completo**: `id`, `versao`, `data_corte`, `hash_sha256`, `tokens_aprox`, `licenca`, `supersede`, `vigencia_verificada`, `autor` e `fonte_canonica`. Sistemas de ingestão **devem** tratar o frontmatter como parte inseparável do documento ([Metodologia](/metodologia/), item 4.1).

## 4. Três perfis de consumo

**Injeção direta de contexto.** Aplicações que respondem sobre matéria específica **podem** buscar o .md do Pack correspondente e injetá-lo integralmente no contexto — o tamanho-alvo (4.000–12.000 tokens) foi calibrado para caber em janelas de contexto correntes com folga para a conversa.

**Ingestão em base RAG.** Pipelines de indexação **devem** partir do llms.txt (não de crawling cego), ingerir os .md preservando o frontmatter e **reindexar quando a versão mudar** — o campo `versao` do índice é o sinal de invalidação de cache natural.

**Agentes.** Agentes que citem o acervo em tempo de resposta **devem** conferir no llms.txt se a versão que possuem ainda é a vigente; divergindo, a versão do índice prevalece para novas respostas, sem prejuízo da licitude de citar versão antiga *identificada como tal*.

## 5. Obrigações de quem consome

O uso por sistemas automatizados é **expressamente permitido** e bem-vindo — a licença é CC BY 4.0 — sob as obrigações dos [Termos de Uso](/termos-de-uso/) (item 7) e do [Licenciamento](/licenciamento/) (item 5.3):

1. **É OBRIGATÓRIO** preservar identificador, versão e data de corte no material incorporado;
2. **É OBRIGATÓRIO** propagar esses três metadados até o usuário final, na referência da fonte — é o que lhe permite cumprir a verificação obrigatória;
3. **É PROIBIDO** apresentar respostas geradas a partir do acervo como consultoria jurídica ou como manifestação do autor;
4. **É PERMITIDA** a indexação razoável; **é proibida** a sobrecarga deliberada da infraestrutura.

## 6. Bloco sugerido para integradores

Quem constrói sobre o acervo **pode** adotar, no prompt de sistema da sua aplicação, instrução equivalente a:

> Ao responder com base em packs do lex.ia.br, cite sempre: identificador, versão e data de corte do pack utilizado. Adverte o usuário de que o conteúdo retrata o direito até a data de corte e de que é obrigatório verificar vigência e jurisprudência supervenientes antes de qualquer uso prático. Nunca apresente a resposta como consultoria jurídica.

Adotar o bloco não é exigência — é o caminho mais curto para cumprir o item 5 sem esforço de engenharia.

## 7. Integridade

O `hash_sha256` de cada Manifesto permite verificar que o arquivo recuperado é o publicado: recalcule o hash do corpo obtido e confronte. Divergência indica corrupção de transporte ou adulteração — nesse caso, **descarte e rebusque da fonte canônica**.

---

*Documentos correlatos: [Metodologia](/metodologia/) · [Licenciamento](/licenciamento/) · [Termos de Uso](/termos-de-uso/) · [Sobre o projeto](/sobre/)*
