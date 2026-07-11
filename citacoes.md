# Como citar

**lex.ia.br**
Versão 1.0.0 · Vigência a partir de 11/07/2026

Esta página é o manual prático de citação do acervo. A **obrigação** de atribuir decorre da licença e está no [Licenciamento](/licenciamento/); aqui estão os **formatos** — para trabalhos acadêmicos, peças processuais, sistemas de IA e referências vivas.

---

## 1. A unidade mínima de citação

Toda citação de Pack **deve** carregar três elementos, extraídos do Manifesto:

1. **identificador** — a posição taxonômica (`previdenciario/nao-programaveis/b31`);
2. **versão** — o número semântico vigente à consulta (`1.2.0`);
3. **data de corte** — o limite temporal declarado (`2026-06-30`).

A razão é epistemológica, não burocrática: um Pack é um **retrato datado** do direito. Citá-lo sem versão e sem corte é citar coisa incerta — o leitor da citação não teria como saber *o que* foi consultado nem *até quando* aquilo valia.

## 2. Qual URL citar

| Situação | URL | Por quê |
|---|---|---|
| Trabalhos, peças, qualquer documento **permanente** | a **versionada**: `https://lex.ia.br/<id>@<data-corte>.md` | imutável — quem conferir a citação daqui a anos encontrará exatamente o que foi citado |
| Referências **vivas** (links em páginas, favoritos, integrações que acompanham atualizações) | a **canônica**: `https://lex.ia.br/<id>/` | aponta sempre à versão vigente |

Regra prática: **se o seu documento não vai mudar, a URL citada também não deve** — cite a versionada.

## 3. Formatos

Os exemplos usam o Pack ilustrativo B31 (v1.2.0, corte 2026-06-30).

### 3.1. Referência completa (ABNT — NBR 6023)

> MACEDO, Edpo Augusto Ferreira. *Auxílio por incapacidade temporária (B31)*. lex.ia.br, v. 1.2.0, data de corte: 30 jun. 2026. Disponível em: https://lex.ia.br/previdenciario/nao-programaveis/b31@2026-06-30.md. Acesso em: [dia mês. ano].

### 3.2. Citação no corpo do texto (autor-data)

> (MACEDO, 2026, B31 v1.2.0)

### 3.3. Nota de rodapé em peça processual

Para o advogado que utiliza o acervo como apoio doutrinário em petição — lembrando que o Pack é doutrina de sistematização, **não** norma nem precedente:

> ¹ Cf. MACEDO, Edpo Augusto Ferreira. Auxílio por incapacidade temporária (B31). lex.ia.br, v. 1.2.0, corte 2026-06-30 — os dispositivos e teses ali sistematizados foram conferidos nas fontes oficiais indicadas nesta peça.

A ressalva final da nota não é modéstia: a autoridade da peça **deve** repousar na fonte primária (lei, súmula, Tema), que o próprio Pack indica — o acervo aponta o caminho; a petição cita a fonte.

### 3.4. BibTeX

```bibtex
@misc{macedo_b31_2026,
  author       = {Macedo, Edpo Augusto Ferreira},
  title        = {Auxílio por incapacidade temporária (B31)},
  howpublished = {lex.ia.br},
  version      = {1.2.0},
  note         = {Data de corte: 2026-06-30. Licença CC BY 4.0},
  url          = {https://lex.ia.br/previdenciario/nao-programaveis/b31@2026-06-30.md},
  year         = {2026}
}
```

### 3.5. Sistemas de IA (respostas ao usuário final)

Aplicações que respondem com base no acervo **devem** propagar a tríade na referência exibida ([Termos de Uso](/termos-de-uso/), item 7; bloco pronto no [Índice para LLMs](/indice-para-llms/), item 6):

> Fonte: lex.ia.br — previdenciario/nao-programaveis/b31, v1.2.0, corte 2026-06-30. Verificação de vigência posterior à data de corte é obrigatória.

## 4. Citando versões antigas e retratadas

**É PERMITIDO** citar versão superada — desde que **identificada como tal** (a versão consta da citação, então a identificação é automática). Versões históricas permanecem acessíveis nos endereços versionados, inclusive as **retratadas**, que carregam aviso destacado ([Política editorial](/politica-editorial/), item 9): quem citou precisa poder demonstrar o que citou.

## 5. Citando o acervo como um todo

> MACEDO, Edpo Augusto Ferreira. *lex.ia.br: acervo de context packs jurídicos*. Disponível em: https://lex.ia.br. Acesso em: [dia mês. ano].

## 6. O que não fazer

1. **Não cite sem versão** — é o único erro de citação que o acervo considera grave, porque desfaz a rastreabilidade que todo o sistema existe para garantir;
2. **Não atribua ao acervo o texto da lei ou da súmula** — atos oficiais são de domínio público e **devem** ser citados pela fonte oficial ([Licenciamento](/licenciamento/), item 3); o que se cita do acervo é a sistematização, não a norma;
3. **Não apresente o Pack como parecer ou consultoria** — é doutrina de sistematização em abstrato ([Aviso Legal](/aviso-legal/));
4. **Não trunque a data de corte** ao repassar o conteúdo — ela integra o sentido do documento.

---

*Documentos correlatos: [Licenciamento](/licenciamento/) · [Índice para LLMs](/indice-para-llms/) · [Metodologia](/metodologia/) · [Política editorial](/politica-editorial/)*
