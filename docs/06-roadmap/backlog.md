# Yresá Governança Global — Backlog de Governança & Padrões Comunitários

> Documento vivo para registro de melhorias na infraestrutura de governança, automações organizacionais do GitHub, templates de issues/PRs e políticas de conformidade do ecossistema Yresá.

---

## Estrutura de Cada Item do Backlog
Cada item registrado neste documento responde a cinco perguntas fundamentais:
1. **O quê?** (Título e resumo claro da ação de engenharia)
2. **Por que fazer?** (Fundamentação arquitetural, proteção de custos ou segurança)
3. **Quando fazer?** (Critério ou gatilho de ativação operacional)
4. **Como fazer?** (Estratégia técnica, arquivos tocados e pacotes)
5. **Critério de Conclusão** (Como sabemos que está pronto e validado)

---

## 📋 Itens Mapeados no Backlog

### [GOV-01] Provisionamento e Parametrização do GitHub Projects v2 da Organização Yresá

* **Status:** In Progress
* **Iniciativa / Épico:** Governança Operacional & Visibilidade Executiva
* **Prioridade:** Alta (Visibilidade Executiva do Ecossistema)
* **Domínios / Módulos Envolvidos:** `github.com/orgs/yresa/projects`
* **Referências:** GitHub Projects v2 API & UI Guidelines.

#### 1. Contexto & Por Que Fazer
O fundador precisa de uma visão panorâmica e em tempo real de todas as ações de engenharia, finanças, infraestrutura e produto sem precisar abrir arquivo por arquivo em 10 repositórios diferentes. O GitHub Projects v2 em nível de organização consolida os 56 itens mapeados em uma única mesa visual.

#### 2. Quando Fazer (Gatilhos de Ativação)
Imediatamente após a publicação dos backlogs normalizados e criação do repositório `yresa/.github`.

#### 3. Como Fazer (Estratégia Técnica)
1. Criar novo projeto em `https://github.com/orgs/yresa/projects/new`.
2. Adicionar visão Board com as colunas: `Backlog`, `In Progress`, `In Review`, `Released`.
3. Adicionar campos customizados `Iniciativa / Épico` e `Prioridade`.
4. Importar ou vincular os itens dos 10 repositórios ao board unificado.

#### 4. Riscos Mitigados
- Previne perda de foco e fragmentação de contexto entre projetos.
- Garante alinhamento imediato antes de iniciar qualquer ciclo de desenvolvimento.

#### 5. Critério de Conclusão
- Painel ativo com visualização Kanban e itens acessíveis em 1 clique na web.

---

### [GOV-02] Padronização Global de Políticas de Segurança (`SECURITY.md`) e Código de Conduta Afetivo

* **Status:** Backlog
* **Iniciativa / Épico:** Conformidade & Segurança da Informação
* **Prioridade:** Média (Conformidade Comunitária)
* **Domínios / Módulos Envolvidos:** `.github/SECURITY.md`, `.github/CODE_OF_CONDUCT.md`
* **Referências:** Diretrizes de Segurança Responsável e Declaração de Vulnerabilidades.

#### 1. Contexto & Por Que Fazer
Centralizar a política de divulgação responsável de vulnerabilidades de segurança (ex: canal seguro para reportar falhas no Gateway ou nos apps) para que pesquisadores de segurança saibam como contatar o time da Yresá sem expor dados de usuários.

#### 2. Quando Fazer (Gatilhos de Ativação)
Antes do lançamento público do aplicativo nas lojas de aplicativos.

#### 3. Como Fazer (Estratégia Técnica)
1. Criar `.github/SECURITY.md` com e-mail criptografado ou canal seguro de reporte.
2. Definir SLAs de resposta para triagem de vulnerabilidades (ex: 48h para primeiro retorno).

#### 4. Riscos Mitigados
- Evita divulgação pública de exploits de segurança antes da correção (*0-day*).

#### 5. Critério de Conclusão
- Arquivo `SECURITY.md` ativo e reconhecido na aba de segurança de todos os repositórios da organização.
