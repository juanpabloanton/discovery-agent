# discovery-agent

# Estructura de archivos
mkdir -p .claude/skills/discovery
mkdir -p .claude/commands/discovery
mkdir -p .claude/hooks
mkdir -p .claude/scripts
mkdir -p discoveries/_template/interviews 
mkdir -p discoveries/_template/outputs
mkdir -p discoveries/citasalud/interviews 
mkdir -p discoveries/citasalud/outputs

# Ejemplo de la clase de la maestria 18/06/2026
https://github.com/bvegaM/discovery-agent


## CLAUDE 
/discovery:analyze discoveries/cienciayfe_secr
/discovery:generate-mvp discoveries/cienciayfe_secr
/discovery:experiments discoveries/cienciayfe_secr
/discovery:report discoveries/cienciayfe_secr


## CODEX CLI

$env:Path = "C:\Users\Juan Pablo\AppData\Local\Programs\OpenAI\Codex\bin;$env:Path"
codex --version


Lee .claude/commands/discovery/analyze.md  O Analiza discoveries/cienciayfe_secr con discovery analyze
Lee .claude/commands/discovery/generate-mvp.md y ejecuta sus instrucciones usando como argumento discoveries/cienciayfe_secr.
Lee .claude/commands/discovery/experiments.md y ejecuta sus instrucciones usando como argumento discoveries/cienciayfe_secr.
Lee .claude/commands/discovery/report.md y ejecuta sus instrucciones usando como argumento discoveries/cienciayfe_secr.