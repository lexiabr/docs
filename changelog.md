# Changelog — registro de versões

**lex.ia.br**
Versão 1.0.0 · Vigência a partir de 11/07/2026

Esta página é a **memória pública do acervo**: o registro cronológico de toda versão fechada, toda supersedência e toda retratação. O llms.txt diz qual é a versão **vigente** de cada Pack; o changelog explica **como se chegou até ela**.

---

## 1. Regras do registro

1. **Toda versão fechada gera entrada** — sem exceção: não existe versão publicada fora do registro;
2. **O registro é append-only** — entradas não se editam nem se removem; corrigir uma entrada é publicar outra que a retifique, com remissão expressa;
3. **Toda alteração declara sua razão suficiente** ([Política editorial](/politica-editorial/), item 8) — o que mudou e por quê: qual lei, qual tese, qual comunicação de erro a motivou;
4. **A ordem é cronológica inversa** — a entrada mais recente no topo;
5. **Comunicações de erro acatadas recebem crédito**, se o comunicante o desejar.

## 2. Como ler uma entrada

Cada entrada carrega, nesta ordem:

| Campo | Conteúdo |
|---|---|
| **Data** | a data do fechamento da nova versão |
| **Pack** | identificador taxonômico, com link para a URL canônica |
| **Transição** | versão anterior → nova versão, com a **natureza** da mudança |
| **Data de corte** | a da nova versão (mantida, em correção material; nova, nas demais) |
| **Razão suficiente** | a motivação de cada alteração, com a fonte |
| **Versões** | links para o .md versionado novo **e** o anterior — os dois permanecem acessíveis |

As quatro naturezas seguem a taxonomia da [Política editorial](/politica-editorial/) (item 6):

- **CORREÇÃO** (patch) — o Pack errava já na sua data de corte; o corte se mantém;
- **SUPERVENIÊNCIA** (minor) — o direito mudou após o corte; corte novo;
- **REESTRUTURAÇÃO** (major) — a mudança inverte a síntese; corte novo;
- **RETRATAÇÃO** — vício de origem; o Pack sai do índice, a URL versionada permanece.

## 3. Modelo de entrada

```markdown
### AAAA-MM-DD · previdenciario/nao-programaveis/b31 · v1.1.0 → v1.2.0 · SUPERVENIÊNCIA

**Data de corte**: 2026-06-30 (anterior: 2026-01-15)

**Razões**:
1. Incorporada a tese firmada no Tema [N]/[Tribunal], julgado em [data],
   que [síntese da tese] — seção II (Antítese) e quadro de DIB na Síntese;
2. Atualizado o valor de [parâmetro administrativo] pela Portaria [N],
   de [data] — tabela de requisitos.

**Crédito**: comunicação de erro de [nome], acatada quanto ao item 2.

**Versões**: [v1.2.0 (vigente)](/previdenciario/nao-programaveis/b31@2026-06-30.md) ·
[v1.1.0 (superseded)](/previdenciario/nao-programaveis/b31@2026-01-15.md)
```

A entrada acima é **modelo ilustrativo** — os dados são fictícios, coerentes com o exemplo B31 usado em toda a documentação do site.

## 4. Consumo por máquinas

O formato das entradas é deliberadamente regular — cabeçalho `data · id · transição · natureza` — para permitir parsing simples. Sistemas de ingestão **podem** monitorar esta página (ou seu feed) para detectar supersedências e invalidar caches; a fonte autoritativa da versão vigente, porém, é sempre o [llms.txt](/indice-para-llms/) — o changelog explica transições, não define estado.

## 5. Registro

*O acervo encontra-se em fase inicial. A primeira entrada será lavrada no primeiro fechamento de versão — e, a partir dela, este registro só cresce.*

<!-- ENTRADAS: inserir novas entradas ABAIXO desta linha, a mais recente primeiro -->

---

*Documentos correlatos: [Política editorial](/politica-editorial/) · [Metodologia](/metodologia/) · [Índice para LLMs](/indice-para-llms/) · [Como citar](/como-citar/)*
