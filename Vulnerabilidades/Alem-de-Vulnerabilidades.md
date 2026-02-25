Mas a caça a bugs (bug bounty) é mais do que apenas saber como XSS ou IDOR funcionam.

Antes de começar a testar alvos reais, você deve se familiarizar com outros conceitos fundamentais que o tornam um caçador completo. Essas habilidades ajudarão você a encontrar mais bugs, evitar erros e se destacar de iniciantes que só conhecem o básico.

Nesta seção, abordaremos:


- [Básicos de Reconhecimento (Recon)](#basicos-de-reconhecimento)
- [Metodologia de teste](#metodologia-de-teste)  
- [Divulgação Responsável e Ética](#divulgacao-responsavel-e-etica)
- [Entendendo Escopos e Regras](#entendendo-escopos-e-regras)
- [Escrita de Relatórios de Bug](#escrita-de-relatorios-de-bug)
- [Mentalidade para Caça de Bugs](#mentalidade-para-caca-de-bugs)


## Básicos de Reconhecimento

Recon é o processo de coletar informações sobre seu alvo antes de testar.

Aqui estão alguns ótimos recursos sobre este tópico:
- [Bug Bounty Recon Guide – YesWeHack](https://www.yeswehack.com/learn-bug-bounty/recon-series-recap-reconnaissance-footprinting)
- [Recon for Bug Bounty: 8 Essential Tools – Intigriti Blog](https://www.intigriti.com/researchers/blog/hacking-tools/recon-for-bug-bounty-8-essential-tools-for-performing-effective-reconnaissance)
- [The Bug Hunter's Methodology v4.0](https://www.youtube.com/watch?v=p4JgIu1mceI)



## Metodologia de teste


Muitos iniciantes testam aleatoriamente, clicando e esperando tropeçar em um bug. Essa abordagem pode funcionar de vez em quando, mas é inconsistente e desperdiça tempo.

Uma metodologia de teste é simplesmente um plano de como você abordará um alvo. Mantém você organizado, reduz áreas perdidas e ajuda a reproduzir resultados.

Este é um exemplo simples que recomendo para iniciantes:

1. **Mapeie a Aplicação**
   - Use a aplicação como um usuário regular usaria.
   - Entenda todas as funcionalidades disponíveis.
   - Liste endpoints, parâmetros e formulários.


2. **Teste Funcionalidade por Funcionalidade**
   - Escolha uma funcionalidade e teste-a para tipos de bugs potenciais, por exemplo, em uma funcionalidade de upload de arquivo, verifique tipos de arquivos irrestritos, path traversal, etc.

3. **Use uma Checklist**
   - Tenha uma lista simples de bugs para verificar. [Este repositório](https://github.com/Az0x7/vulnerability-Checklist?tab=readme-ov-file) é um bom ponto de partida.
   - Atualize sua checklist à medida que aprende mais.

4. **Tome Notas**
   - Documente o que testou, o que funcionou, comportamentos interessantes, etc.
   - Use [Obsidian](https://obsidian.md/) ou [Notion](https://www.notion.com/)



## Divulgação Responsável e Ética

Bug bounty hunting só funciona quando há confiança entre caçadores e organizações. Essa confiança vem de seguir as regras e agir responsavelmente.

Mantenha estes princípios em mente:

1. **Apenas teste alvos para os quais você tem permissão.** - Apenas teste alvos listados como "in-scope" (no escopo).
   - Nunca teste sites aleatórios, é ilegal e pode ter sérias consequências.

2. **Relate, não explore.** - Seu objetivo é provar que o bug existe, não causar danos.  
   - Evite ações que possam prejudicar dados, usuários ou sistemas.

3. **Siga regras de divulgação.** - Alguns programas permitem writeups públicos após uma correção, outros exigem confidencialidade permanente. Sempre respeite a política de divulgação do programa.

4. **Seja profissional.** - Forneça comunicação clara e respeitosa.  
   - Evite frustração ou hostilidade, mesmo se seu relatório for marcado como duplicado ou N/A.


## Entendendo Escopos e Regras

Antes de testar qualquer coisa, você precisa saber exatamente o que tem permissão para hackear. É isso que o escopo e as regras definem.

As diretrizes do programa dizem quais alvos você pode testar, quais tipos de vulnerabilidades estão no escopo e quais métodos de teste são permitidos. Muitas regras são comuns em programas de bug bounty, mas alguns programas também têm requisitos únicos.

Aqui está o que você deve saber sobre escopo e regras:

1. **Básicos de Escopo**
   - **In-scope** significa que você tem permissão para testar esses alvos.  
   - **Out-of-scope** significa que você deve evitá-los completamente.  
   - O escopo pode incluir domínios, subdomínios, faixas de IP, aplicativos móveis, APIs e mais.  

2. **Lendo o Escopo com Cuidado**
   - Procure por listas de alvos, curingas (wildcards) e exclusões.  
   - Preste atenção a notas que especificam ambientes de teste ou restrições.  
   - Alguns programas limitam os tipos de vulnerabilidades que aceitam.  

3. **Regras para Seguir**
   - Sem ataques de negação de serviço (DoS).  
   - Sem spam ou phishing de usuários.  
   - Evite varreduras automatizadas que possam sobrecarregar sistemas.  
   - Não acesse ou modifique dados reais de clientes.  





## Escrita de Relatórios de Bug

Encontrar um bug é apenas metade do trabalho. Se seu relatório for pouco claro ou incompleto, a equipe de segurança do programa pode rejeitá-lo, julgar mal seu impacto ou pedir para refazer o trabalho.

Um bom relatório de bug deve ser claro, conciso e reproduzível.

Aqui está o que todo bom relatório de bug deve incluir:

1. **Título**
   - Mantenha curto mas descritivo.  
   - Exemplo: "IDOR em /api/user permite acesso à informação de outros usuários."

2. **Descrição**
   - Explique claramente o que é o bug e por que ele importa.  
   - Inclua o tipo de vulnerabilidade, o endpoint ou funcionalidade afetada e o impacto potencial.

3. **Passos para Reproduzir**
   - Escreva instruções passo-a-passo para que qualquer um possa replicar o problema.  
   - Mantenha cada passo claro e em ordem.  
   - Inclua payloads de exemplo ou requisições modificadas onde necessário.

4. **Impacto**
   - Explique o que um atacante poderia fazer se esse bug fosse explorado.  
   - Conecte-o a consequências do mundo real como roubo de dados, tomada de conta ou interrupção de serviço.

>[!Note] 
>Eu criei um GPT chamado [ReportWriter](https://chatgpt.com/g/g-67adbeb78b588191aeadae88489173d9-report-writer) para tornar essa tarefa mais fácil. Use [ReportWriter](https://chatgpt.com/g/g-67adbeb78b588191aeadae88489173d9-report-writer) para ajudar a escrever relatórios claros e estruturados.



## Mentalidade para Caça de Bugs

Bug bounty hunting é um jogo de longo prazo. Você não encontrará bugs críticos todos os dias, e enfrentará rejeições, duplicatas e períodos de seca. Sua mentalidade frequentemente decidirá se você melhora ou desiste.

As dicas a seguir podem ajudar você a se manter motivado e melhorar com o tempo:

1. **Seja Paciente**
   - Bugs de alta qualidade levam tempo para encontrar. Não espere recompensas instantâneas.  
   - Trate cada sessão de teste como prática, mesmo se não encontrar nada.

2. **Mantenha-se Curioso**
   - Há sempre algo para aprender se você for curioso o suficiente.  
   - Explore partes de uma aplicação que outros podem ignorar.

3. **Pense Como um Desenvolvedor**
   - Entenda como funcionalidades são construídas e como a aplicação deve funcionar.  
   - Considere quais pequenas verificações ou validações um desenvolvedor pode ter perdido.


4. **Aprenda com Cada Relatório**
   - Leia writeups de outros caçadores para ver diferentes abordagens. Recomendo fortemente ler cada relatório divulgado nos programas [Shopify](https://hackerone.com/shopify) e [GitLab](https://hackerone.com/gitlab).
   - Analise suas próprias rejeições ou duplicatas para melhorar na próxima vez.

5. **Seja Consistente**
   - Caçar regularmente constrói habilidades mais rápido do que sessões maratona raras.  
   - Mesmo sessões de prática curtas e focadas importam.

6. **Proteja Sua Saúde Mental**
   - Sua saúde é muito mais importante do que bug bounties ou dinheiro.  
   - [Este vídeo](https://www.youtube.com/watch?v=raH7tRy8M7g) oferece conselhos úteis sobre manter sua saúde mental.

7. **Você só encontrará o que estiver procurando** - Se você quer encontrar bugs de alta severidade, você tem que ativamente caçar por eles.  
     Se passar todo seu tempo testando frutas baixas como open redirects ou problemas de DKIM, não espere tropeçar em um IDOR ou SSRF. Foque seus esforços onde quer resultados.