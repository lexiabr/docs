# Política editorial e de correções

**lex.ia.br**
Versão 1.0.0 · Vigência a partir de 11/07/2026

---

## 1. Objeto

Esta Política disciplina a **governança editorial** do acervo: o que entra, por quais critérios, sob qual hierarquia de fontes, e — sobretudo — **como se classificam e se remediam as alterações**. Ela não repete a [Metodologia](/metodologia/), que rege a fabricação de cada Pack (anatomia, regra epistêmica, ciclo de fechamento): a Metodologia diz *como se faz um documento*; esta Política diz *como se governa o acervo*.

## 2. Seleção de matérias

O acervo cresce por **curadoria**, não por varredura. Uma matéria é elegível quando reúne, cumulativamente:

1. **relevância social** — alta demanda real de informação (benefícios, direitos de massa, institutos de uso cotidiano);
2. **alta taxa de erro em respostas de IA** — matérias em que assistentes frequentemente alucinam requisitos, prazos ou teses são prioritárias, porque é nelas que um documento recuperável rende mais;
3. **maturidade suficiente da controvérsia** — matéria em reforma legislativa em curso ou com tese vinculante pendente de publicação **pode** ser adiada, ou publicada com as pendências marcadas, mas **não deve** ser publicada simulando estabilidade que não existe.

A recusa também é ato editorial: matéria fora do escopo, ou que exigiria simular certeza, **não entra** — a lacuna declarada do acervo vale mais que a cobertura aparente.

## 3. Hierarquia de fontes

Na fabricação e na correção dos Packs, as fontes obedecem a precedência estrita:

1. **Fontes primárias oficiais** — texto legal no Planalto/DOU, inteiro teor e teses nos portais dos tribunais (STF, STJ, TNU, TST), atos administrativos na origem;
2. **Fontes vinculantes sistematizadas** — súmulas, Temas de repetitivos e de repercussão geral, enunciados de observância obrigatória;
3. **Doutrina** — referida como opinião, jamais como norma.

**É PROIBIDO** fundar afirmação normativa em agregadores, portais de notícias jurídicas ou compilações não oficiais sem confirmação na fonte primária — a fonte secundária **pode** apontar o caminho; **não pode** sustentar a afirmação.

## 4. Revisão

O acervo é obra de **autor único** ([Autor](/autor/)), e esta Política não finge colegiado inexistente. A confiabilidade decorre de **revisão procedimental**, não de pluralidade de revisores:

1. as **travas de fechamento** da Metodologia (proibido fechar com pendência de verificação; campo *vigência verificada* preenchido item a item);
2. a **auditabilidade externa** — todo leitor tem acesso à mesma fonte primária citada e ao canal de comunicação de erros (item 7), que funciona como revisão por pares permanente e aberta;
3. a **imutabilidade verificável** — o sha-256 garante que o que se audita é o que foi publicado.

## 5. Independência e conflitos de interesse

1. **Nenhum Pack é patrocinado.** A publicidade exibida no site é de terceiros, identificada como "Publicidade", sem ingerência sobre pauta ou texto;
2. **Packs tratam matérias em abstrato** — jamais casos concretos do escritório, de clientes ou de adversários; a coincidência entre matéria de Pack e matéria advocatícia do autor é natural (escreve-se sobre o que se domina) e não constitui, por si, conflito;
3. Sobrevindo interesse concreto capaz de comprometer a isenção sobre determinada matéria, o Pack correspondente **deve** declará-lo em nota ou ser confiado a fonte diversa.

## 6. Taxonomia das alterações — o que dispara nova versão

Pack publicado **não se edita** ([Metodologia](/metodologia/), item 2). Toda mudança é **nova versão**, e o versionamento semântico (X.Y.Z) classifica sua natureza:

| Natureza | O que é | Versão | Data de corte |
|---|---|---|---|
| **Correção material** (PATCH) | o Pack afirmava algo **errado já na sua data de corte** — dispositivo mal citado, número de Tema trocado, requisito inexistente | X.Y.**Z+1** | mantida |
| **Superveniência** (MINOR) | o Direito **mudou após o corte** — lei nova, tese firmada, modulação — sem inverter a estrutura da síntese | X.**Y+1**.0 | **nova** |
| **Reestruturação** (MAJOR) | a mudança **inverte a síntese** — entendimento vinculante superado, instituto reformado na essência, taxonomia realocada | **X+1**.0.0 | **nova** |
| **Aperfeiçoamento editorial** | clareza, estilo, formatação, **sem alteração de sentido** | acumula para a próxima versão de qualquer natureza | — |

Duas consequências práticas: (a) **correção material é a única hipótese que preserva a data de corte** — corrige-se o retrato, não se tira retrato novo; (b) aperfeiçoamento editorial **nunca** justifica versão própria nem, muito menos, edição silenciosa — acumula e sai carona na próxima.

## 7. Comunicação de erros

Qualquer pessoa **pode** comunicar erro pelo canal indicado na página de [Contato](/contato/), observando os três requisitos da comunicação fundamentada (identificador + versão; trecho; fundamento com fonte primária).

O compromisso editorial:

1. **exame** da comunicação em prazo razoável — como regra, até **[N] dias úteis**;
2. **resposta** ao comunicante, com o juízo: erro confirmado (e a versão corretiva programada), divergência de interpretação (registrável como antítese, se relevante) ou improcedência fundamentada;
3. **crédito** ao comunicante no changelog, se ele o desejar — a revisão aberta merece reconhecimento;
4. divergência interpretativa razoável **não é erro**: **pode** ensejar o enriquecimento da antítese do Pack em versão futura, nunca "correção" que apague a controvérsia.

## 8. Changelog e razão suficiente

Toda nova versão publica changelog sintético em que **cada alteração declara sua razão suficiente** — o que mudou e **por quê** (qual fonte, qual comunicação, qual superveniência a motivou). Alteração sem razão declarada não deve existir; se não se consegue justificá-la, não se deveria tê-la feito.

## 9. Retratação

Identificado vício de origem que comprometa o Pack como um todo — e não apenas trecho corrigível — o documento é **retratado**: sai do índice e da URL canônica, recebe aviso destacado de retratação, **mas a URL versionada permanece acessível**. O acervo não pratica apagamento: quem citou a versão retratada precisa poder demonstrar o que citou. A retratação é, ela própria, registrada no changelog com sua razão suficiente.

## 10. Ferramentas de IA

O papel e os limites da IA na produção estão fixados na [Metodologia](/metodologia/) (item 7) e na página do [Autor](/autor/): apoio à pesquisa e ao rascunho, **sim**; fixação de data de corte, resolução de pendências, decisão de controvérsias e assinatura, **não** — atos humanos indelegáveis do responsável editorial.

## 11. Alterações desta Política

Esta Política **pode** ser atualizada; cada versão é identificada por número e data de vigência no topo. Mudança de critério editorial **não retroage**: Packs publicados permanecem regidos pelas regras vigentes à época de seu fechamento. **Não se deve presumir** a imutabilidade do texto.

---

*Documentos correlatos: [Metodologia](/metodologia/) · [Autor](/autor/) · [Contato](/contato/) · [Termos de Uso](/termos-de-uso/)*
