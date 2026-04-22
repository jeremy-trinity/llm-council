# folderguide.md — github\llm-council\
# Ficheiro de orientação para Claude. Ler antes de trabalhar neste repo.
# VERIFICAR E ACTUALIZAR: pedir a outra conta para confirmar o que falta ou está errado.
# Última actualização: 2026-04-22

---

## O QUE É ESTE PROJECTO

Web app local que envia queries a múltiplos LLMs em paralelo via OpenRouter,
faz revisão cruzada anónima entre eles, e um "Chairman" LLM sintetiza a resposta final.

**Stack:** Python backend (uv) + React/Vite frontend
**Correr:** `./start.sh` ou backend + frontend em terminais separados
**API:** OpenRouter (chave em .env)

---

## PARA QUE SERVE NO CONTEXTO DO JEREMY

Usado para análises de alta qualidade quando uma única LLM não é suficiente.
Já foi usado para:
- Analisar a sequência de 4 emails de candidatura às universidades americanas
  (resultado em `D:\claudeui\CouncilAnalysisResult_2026-04-20.txt`)
- Avaliar deliverability e estratégia da campanha de email

Próximo uso previsto:
- Analisar variações do email para evitar fingerprint de spam (quando iniciar warm-up)
- Avaliar CVs e cover letters antes de enviar

---

## ESTADO ACTUAL

O README diz "99% vibe coded" e "sem suporte activo". Isso significa:
- Funciona mas não tem testes
- Não está em produção contínua — corres quando precisas, fechas quando acabas
- Não tem deploy cloud — é sempre local

---

## VERIFICAR — estado real a 2026-04-22:
- [x] Usado após 2026-04-20? NÃO — sem novos ficheiros de análise no workspace
- [x] Novos ficheiros de análise para rules-and-context? NÃO — só existe CouncilAnalysisResult_2026-04-20.txt (e uma cópia não documentada na raiz)
- [ ] Chave OpenRouter válida com créditos? NÃO VERIFICÁVEL localmente

Última verificação: 2026-04-22
