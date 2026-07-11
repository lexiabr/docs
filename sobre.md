# Sobre o projeto

**lex.ia.br**
Versão 1.0.0 · 11/07/2026

---

## Em uma frase

O **lex.ia.br** é um acervo de **packs de contexto jurídico**: unidades documentais de Direito brasileiro, curadas, versionadas e com **data de corte declarada**, escritas para serem lidas por pessoas **e** consumidas por sistemas de inteligência artificial.

## O problema

A informação jurídica brasileira é abundante e dispersa: leis emendadas dezenas de vezes, jurisprudência que se consolida e se revê, teses vinculantes com modulação de efeitos, portarias que reescrevem o procedimento sem tocar na lei. Quem pesquisa — pessoa ou máquina — raramente encontra a matéria **inteira** em um lugar só: encontra fragmentos, cada um com idade diferente e nenhum dizendo qual é a sua.

Para sistemas de IA, o problema se agrava. Modelos de linguagem respondem sobre Direito com fluência e, com a mesma fluência, misturam a redação atual com a revogada, a súmula vigente com a cancelada. Aplicações RAG mitigam o risco recuperando documentos — mas herdam a qualidade do que recuperam: se a base é um agregado de fragmentos sem data, a resposta é um agregado de incertezas sem data.

## A tensão

A resposta usual do mercado é prometer **atualização permanente** — "conteúdo sempre atualizado". A promessa é epistemicamente desonesta: nenhuma base acompanha, em tempo real, todas as fontes do Direito; toda base dinâmica está desatualizada em algum ponto, **sem dizer em qual**. A desatualização silenciosa é pior do que a desatualização declarada, porque desarma a diligência de quem lê.

## A resposta

O lex.ia.br inverte a promessa. Em vez de fingir atualidade, cada pack **declara seus limites**:

- **Estático** — o pack retrata a matéria até a sua **data de corte**, e apenas até ela. Não muda por baixo do leitor;
- **Versionado** — mudanças geram nova versão, com registro de supersedência; a versão antiga permanece citável como versão antiga;
- **Verificável** — o manifesto de cada pack registra identificador, versão, data de corte, licença, autoria e soma de verificação (sha-256);
- **Estruturado** — a matéria é exposta em **tese** (base normativa e o entendimento consolidado), **antítese** (controvérsias, exceções e entendimentos divergentes) e **síntese** (o estado da questão, quadros operacionais, termos iniciais e prazos);
- **Regido** — todo pack carrega o mesmo regime de uso: **é obrigatório** verificar a vigência após a data de corte; **é proibido** presumir a atualidade.

A honestidade sobre o limite é o que torna o acervo confiável: o leitor — humano ou máquina — sabe exatamente o que está garantido e a partir de onde começa a sua própria diligência.

## Para quem

- **Advogados e estudantes** — packs como ponto de partida sistematizado de uma matéria: a estrutura dialética entrega a norma, a divergência e o estado da questão em leitura única;
- **Desenvolvedores de sistemas jurídicos de IA** — unidades de contexto delimitadas, com metadados de proveniência e licença clara ([CC BY 4.0](/licenciamento/)), prontas para ingestão em bases RAG;
- **Pesquisadores** — corpus versionado e citável, em que cada afirmação tem data.

## Como usar

**Lendo.** A página inicial é o motor de busca do acervo, com filtros por categoria e tag. A [árvore de categorias](/arvore/) exibe os ramos do Direito hierarquizados — o gênero contendo suas espécies — e o [tesauro](/tesauro/) lista o vocabulário completo de tags.

**Integrando.** Cada pack expõe seu arquivo-fonte em markdown (.md) com o manifesto em frontmatter, e o índice para LLMs ([llms.txt](/llms.txt)) enumera o acervo em formato legível por máquinas. As condições estão na página de [Licenciamento](/licenciamento/) — em resumo: uso livre com atribuição, **preservados identificador, versão e data de corte**.

## O ecossistema

O lex.ia.br integra um conjunto de projetos de estruturação do conhecimento jurídico mantidos pelo mesmo autor, ao lado da enciclopédia **Ratio Decidendi** (verbetes ontológicos de conceitos jurídicos) e de iniciativas de ensino em Direito Previdenciário. Cada projeto tem função própria: a enciclopédia define conceitos; o lex.ia.br entrega matérias operacionais delimitadas no tempo.

## Quem mantém

O projeto é mantido por **Edpo Ferreira Macedo**, advogado (OAB/SP 489.672), sob a **Ferreira Macedo Sociedade Individual de Advocacia** — atuação em Direito Previdenciário, do Trabalho e Civil. Perfil completo na página do [Autor](/autor/).

O método editorial — critérios de curadoria, ciclo de versão, o que dispara revisão — está descrito na página de [Metodologia](/metodologia/).

## Documentos do site

[Termos de Uso](/termos-de-uso/) · [Aviso Legal](/aviso-legal/) · [Política de Privacidade](/politica-de-privacidade/) · [Política de Cookies](/politica-de-cookies/) · [Licenciamento](/licenciamento/)

---

*Contato: **contato@lex.ia.br***
