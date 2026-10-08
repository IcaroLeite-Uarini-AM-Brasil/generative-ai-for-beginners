# Checklist de documentação e tradução PT-BR

## Status da correção crítica

- [x] Corrigir referências inválidas de modelo `gpt-5-mini` em exemplos do currículo
- [x] Atualizar exemplos de código para `gpt-4o-mini` quando aplicável
- [x] Corrigir a lógica de re-ranking no módulo de RAG
- [x] Validar o conteúdo dos READMEs principais afetados

## Revisão de traduções PT-BR

### Prioridade 1 (alta visibilidade)
- [ ] Lesson 04 — Prompt Engineering Fundamentals
- [ ] Lesson 06 — Text Generation Applications
- [ ] Lesson 07 — Building Chat Applications
- [ ] Lesson 15 — RAG and Vector Databases

### Prioridade 2 (complementares)
- [ ] Lesson 01 — Introduction to Generative AI
- [ ] Lesson 02 — Exploring and Comparing Different LLMs
- [ ] Lesson 03 — Using Generative AI Responsibly
- [ ] Lesson 05 — Advanced Prompts

## Checklist documental

- [ ] Confirmar que os READMEs principais têm exemplos consistentes em todo o curso
- [ ] Padronizar nomes de modelos e configurações de ambiente
- [ ] Revisar tabelas comparativas para clareza do leitor
- [ ] Incluir instruções de troubleshooting em lições com código de API
- [ ] Verificar URLs e tracking em links de documentação Microsoft
- [ ] Garantir que entradas de código e snippets estejam em sintaxe válida
- [ ] Verificar que os exemplos de prompts e saídas são coerentes com o modelo usado

## Observações de revisão

1. A correção crítica anterior foi baseada no fato de que o modelo `gpt-5-mini` foi atualizado no currículo upstream, mas o fork em estudo ainda apresentava referências inconsistentes.
2. O padrão atual recomendado para a base de exemplos é usar modelos validados e consistentes em todo o curso.
3. Traduções em PT-BR devem preservar termos técnicos sem perder precisão, especialmente em RAG, embeddings, chat applications e prompt engineering.

## Próximo passo recomendado

- [ ] Finalizar revisão textual das lições prioritárias em PT-BR
- [ ] Abrir PR com escopo de correção crítica + documentação
- [ ] Validar se a branch está sincronizada com a base upstream antes do merge
