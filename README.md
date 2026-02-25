# Primeira Recompensa

## Introdução

> [!Note]
> O objetivo deste guia é levar alguém de zero conhecimento em bug bounties e segurança de aplicações web para ganhar sua primeira recompensa (prêmio em dinheiro).

A maioria das pessoas estão perdidas e sobrecarregadas pela infinita lista de recursos disponíveis.

Acho que há dois problemas principais com a maioria desses recursos:

- Esquecem que o leitor é um iniciante que apenas quer um ponto de partida claro
- Acreditam que adicionar mais ferramentas, links e palavras-chave torna o guia mais valioso

Quero resolver esses problemas.

Uma coisa a ter em mente é que todos pensam diferente. Pessoas têm diferentes estilos de aprendizado e abordagens, então você pode encontrar outros roteiros ou conselhos que sugerem um caminho diferente. Isso é totalmente normal.

Quando comecei, tive que aprender tudo por tentativa e erro. Desperdicei semanas indo na direção errada.

Este repositório é minha forma de ajudá-lo a pular as adivinhas e construir uma base forte. Uma vez que você tenha o básico, evoluir será muito mais fácil.

## 🌐 1. Fundamentos da Web

O que separa alguém ganhando $250K por ano em bug bounties de alguém que nem consegue encontrar um bug válido é **conhecimento**.
Quanto mais você souber, melhor será seu desempenho.

Se você vai hackear aplicações web, é muito útil entender como aplicações web modernas são construídas e como funcionam.

Para esta primeira fase, não vou lhe entregar recursos diretos.

Por quê? Porque essa abordagem ajudará você a construir habilidades de alto valor a longo prazo:

- Resolução de problemas por conta própria
- A capacidade de explorar e aprender novas habilidades
- Paciência

O único dica que vou dar é: procure no Google ou pergunte ao ChatGPT.

**Caminho para Aprender Fundamentos da Web:**

1. **Noções Básicas de HTML e CSS**
   - Entenda como as páginas web são estruturadas e estilizadas.

2. **Fundamentos de JavaScript**
   JavaScript é a linguagem de programação da web. Aprenda o básico como variáveis, funções e eventos, é fundamental para encontrar bugs como XSS.
   - Quanto mais JavaScript você aprender, mais oportunidades terá. Com certeza compensará a longo prazo..

3. **Conceitos Principais do React.js**
   React é um framework JavaScript para construir UIs dinâmicas. Aprender seus básicos o ajudará a entender como dados fluem em aplicações modernas, identificar vulnerabilidades do lado do cliente e testar o comportamento dos componentes efetivamente.
   - Entenda componentes, props, state e como dados fluem em uma aplicação React.

4. **Fundamentos do Next.js**
   Next.js é um framework baseado em React para aplicações full-stack que combinam capacidades frontend e backend em um projeto.
   Suporta recursos como renderização no servidor, rotas de API e roteamento baseado em arquivos, tornando muito útil para entender como aplicações web modernas funcionam.

   Foco em entender roteamento, componentes do servidor e arquitetura baseada em arquivos.
   Certifique-se de aprender bem essas três áreas:

   - **Sistemas de autenticação:** Como cookies, JWT e OAuth funcionam
   - **Bancos de dados:** Como armazenar, consultar e gerenciar dados usando SQL
   - **APIs:** Como requisitar, recuperar e enviar dados para APIs. Use ferramentas como [Postman](https://www.postman.com/) e aprenda HTTP básico

## 🐞 2. Vulnerabilidades

Depois de aprender como aplicações web são construídas e como funcionam, invadir será muito mais fácil.

Nesta seção, focaremos em aprender os tipos de bugs que você provavelmente encontrará em programas de bug bounty.

Para aprender um tipo de bug bem, seguiremos este processo:

1. Estude os básicos da vulnerabilidade
2. Pratique o que aprendeu para solidificar seu entendimento dos básicos.
3. Leia relatórios reais de bug bounty para entender:
   - Como outros estão encontrando esse tipo de bug
   - Onde é mais provável existir
   - Como é explorado
   - Como o impacto no mundo real parece

> [!Note]
> A maioria dos desafios e CTFs que você resolverá serão muito mais fáceis do que encontrar o mesmo tipo de bug em um alvo real. Isso ocorre porque aplicações web modernas têm mais proteções, e muitos outros caçadores de bugs podem já ter testado as mesmas áreas.

> [!Tip]
> Em muitos relatórios, você encontrará correntes de múltiplas vulnerabilidades. Se ver um bug que ainda não estudou, não se preocupe, chegará a ele depois. Sempre pode pausar, aprender esse bug da lista e depois voltar ao relatório. A ordem aqui não é rígida.

**Aqui está seu guia:**

- [Antes de Começar](https://github.com/PedrooHSN-Dev/First-Bounty-PT/blob/main/Vulnerabilidades/Antes-de-Comecar.md)
- [Bugs de Injeção](https://github.com/PedrooHSN-Dev/First-Bounty-PT/blob/main/Vulnerabilidades/Bugs-de-Injecao.md)
- [Bugs de Lógica do Lado do Servidor](https://github.com/PedrooHSN-Dev/First-Bounty-PT/blob/main/Vulnerabilidades/Bugs-de-Logica-do-Lado-do-Servidor.md)
- [Bugs do Lado do Cliente](https://github.com/PedrooHSN-Dev/First-Bounty-PT/blob/main/Vulnerabilidades/Bugs-do-Lado-do-Cliente.md)
- [Bugs de Autenticação](https://github.com/PedrooHSN-Dev/First-Bounty-PT/blob/main/Vulnerabilidades/Bugs-de-Autenticacao.md)
- [Bugs de Autorização](https://github.com/PedrooHSN-Dev/First-Bounty-PT/blob/main/Vulnerabilidades/Bugs-de-Autorizacao.md)
- [Bugs de Configuração de Infraestrutura](https://github.com/PedrooHSN-Dev/First-Bounty-PT/blob/main/Vulnerabilidades/Bugs-de-Configuracao-de-Infraestrutura.md)
- [Além de Vulnerabilidades](https://github.com/PedrooHSN-Dev/First-Bounty-PT/blob/main/Vulnerabilidades/Alem-de-Vulnerabilidades.md)

## 🚀 3. Começando com Hacking Real

Depois de aprender os fundamentos da web, vulnerabilidades comuns e entender as regras, é hora de colocar tudo em ação.

O objetivo aqui é começar a caçar em um ambiente real para que você possa aplicar o que aprendeu e trabalhar para ganhar sua primeira recompensa.

- Cadastre-se em [HackerOne](https://hackerone.com/).
- Escolha um alvo do [diretório](https://hackerone.com/directory/programs).
> [!Tip]
> Quanto mais relatórios um programa resolveu, maior suas chances de encontrar um bug como iniciante.
- Comece a caçar usando nossa [metodologia de teste](https://github.com/PedrooHSN-Dev/First-Bounty-PT/blob/main/Vulnerabilidades/Alem-de-Vulnerabilidades.md#metodologia-de-teste)
- Mantenha foco no seu alvo por pelo menos 6–8 semanas.

Depois dessas 6–8 semanas, você deve ter uma chance sólida de ganhar sua primeira recompensa.



## 🧰 4. Habilidades de Apoio

Não importa onde você está em sua jornada, dedique tempo para aprender e explorar novas áreas.
Como iniciante, existem algumas habilidades extras que vale a pena aprender cedo e compensarão depois.

### Redes
Redes é a base de como dispositivos e sistemas se comunicam pela internet. Entendê-lo ajuda você a fazer sentido de como dados se movem entre clientes, servidores e outros sistemas.
Por enquanto, foque no básico como endereçamento IP, DNS e como dispositivos se conectam e comunicam.

Recursos:
- [Introdução às Redes – Zero to Mastery](https://zerotomastery.io/blog/introduction-to-networking/)
- [Fundamentos de Redes PDF](https://www.ece.uvic.ca/~itraore/elec567-13/notes/dist-03-4.pdf)

### Noções Básicas de Linux
Linux é o sistema operacional que alimenta a maioria dos servidores e muitas ferramentas de segurança. É importante porque muitos passos de exploração no mundo real, desde executar scripts até analisar logs, são mais fáceis e rápidos em um ambiente Linux.
Você não precisa ir fundo por enquanto, apenas aprenda comandos básicos, navegação de arquivos e permissões.

Recursos:
- [Linux Journey](https://linuxjourney.com/)
- [OverTheWire: Bandit](https://overthewire.org/wargames/bandit/)

### Python ou Go
Python e Go são ótimos para automatizar tarefas e construir ferramentas de hacking.
Conhecer um ajudará você a processar dados mais rápido, construir ferramentas personalizadas e automatizar tarefas repetitivas.

Recursos:
- [Automate the Boring Stuff with Python](https://automatetheboringstuff.com/) / [Learn Python](https://www.learnpython.org/)
- [Go by Example](https://gobyexample.com/)

## 💡 FAQ

### Quanto tempo leva aprender tudo isso?
Depende de quanto tempo você dedica e sua experiência prévia. Acredito que começando do zero e seguindo este roteiro consistentemente, é possível ganhar uma primeira recompensa dentro de 6–8 meses.

---

### Vale a pena bug bounty?
Sim, se você gosta de aprender, resolver problemas e persistência.

Não, se está procurando dinheiro rápido ou um caminho fácil.

---

### Bug bounty é fácil?
Não. Os básicos são simples de entender, mas encontrar bugs impactantes leva paciência, habilidade e criatividade.
Se está procurando "fácil", bug bounty não é para você, mas é exatamente o desafio que o torna tão gratificante.

---

### Sou bom em CTFs e desafios mas não consigo encontrar bugs. O que devo fazer?
CTFs testam resolução de problemas em ambientes controlados. Alvos reais de bug bounty são bagunçados, imprevisíveis e não lhe dão dicas. Comece a aplicar suas habilidades a aplicações reais, mantenha foco e vá mais fundo. Eventualmente, encontrará seu primeiro bug válido.

---

### Continuo abandonando programas/alvos. O que devo fazer?
Comprometa-se com um alvo por pelo menos 6–8 semanas. Abandonar cedo significa que nunca chega aos bugs mais profundos. Trate cada alvo como um quebra-cabeça de longo prazo em vez de um golpe rápido.

---

### Os bugs nos relatórios parecem tão fáceis, mas meus alvos parecem seguros. Por quê?
Você está vendo a história final e polida. O caçador provavelmente passou dias ou semanas explorando antes de encontrar aquele bug "fácil". Segurança não é absoluta mas encontrar a lacuna leva persistência e o ângulo certo.

---

### Existem muitos recursos por aí. Por onde devo começar?
Comece com o roteiro neste repositório. Siga passo a passo para evitar sobrecarga.

---

### Devo esperar aprender toda categoria de bug antes de começar a caçar?
Não. Você nunca realmente "terminará" de aprender todas as categorias de bugs; até caçadores experientes ainda estão aprendendo.
Assim que aprender um tipo de bug, você pode começar a aplicá-lo a alvos reais. Mesmo que não encontre nada, você se familiarizará com o processo e ganhará experiência.

---

### Como posso ver o que outros estão fazendo?
Participe de comunidades de bug bounty no X, Reddit e Discord. Siga caçadores ativos, leia seus posts e relatórios, e participe das discussões.

Aqui estão algumas comunidades que valem a pena verificar:
- [r/bugbounty](https://www.reddit.com/r/bugbounty/)
- [Bug Bounty Write-Ups](https://x.com/i/communities/1489229152280530960)

---

### Quais ferramentas você usa?
Minha ferramenta principal é Burp Suite, mas também uso:
- [ffuf](https://github.com/ffuf/ffuf)
- [nuclei](https://github.com/projectdiscovery/nuclei)
- [waybackurls](https://github.com/tomnomnom/waybackurls)
- [LinkFinder](https://github.com/GerbenJavado/LinkFinder)
- [Arjun](https://github.com/s0md3v/Arjun)
- [cloud_enum](https://github.com/initstring/cloud_enum)

## ⚠️ Erros Comuns de Iniciantes para Evitar

Como iniciante, você não saberá de tudo — e isso é normal.
O objetivo aqui é evitar erros que desperdiçam tempo e causam frustração, então você pode focar nas coisas certas e continuar melhorando a longo prazo.

- **Não trabalhe 24/7**
  Este campo pode ser viciante. Se trabalhar demais, você queimará rápido. Tire pausas e se organize.
  Não recomendo trabalhar nos fins de semana ou mais de 8 horas por dia.

- **Não instale Kali Linux (apenas porque é "para hacking")**
  Kali é apenas uma distro Linux com muitas ferramentas pré-instaladas. É legal, mas desnecessário. Recomendo usar uma distro estável como Ubuntu e instalar apenas as ferramentas que você realmente precisa.

- **Não fique obcecado com ferramentas**
  Existem inúmeras ferramentas por aí. Não as colecione apenas por coletar. Fique com as que funcionam para você.

- **Não se compare com outros**
  A jornada de cada um é diferente. Foque no seu próprio progresso. Você pode aprender e dominar este campo com tempo e prática suficientes.

- **Quando vir uma recompensa de alguém, não fique emocional**
  Use como motivação, não como razão para ficar desanimado. Continue melhorando suas habilidades e você ganhará recompensas altas.

- **Tenha uma visão**
  Depois de um tempo, você pode perder motivação ou entusiasmo. Ter um objetivo claro de longo prazo ajudará você a se manter focado.
  Não faça apenas por dinheiro, você está em um campo que pode ter um impacto positivo significativo em milhões de usuários.

- **Pense e procure antes de fazer perguntas**
  Frequentemente, a resposta já está lá. Procurar primeiro o tornará um melhor aprendiz e ajudará você a evitar parecer um novato.

- **Fique com o que funciona para você**
  Não pule constantemente entre diferentes abordagens ou tipos de bugs. Dê tempo para sua estratégia produzir resultados.

- **Não leve as coisas para o lado pessoal**
  Infelizmente, há pessoas tóxicas neste campo. Se alguém responder mal a suas perguntas de iniciante, passe adiante e foque naqueles que ajudam.

- **Não faça spam com outras pessoas**
  Respeite o tempo e espaço das pessoas. Enviar DMs ou emails constantemente fará com que ignorem suas perguntas.

- **Não pare de aprender**
  Bug bounty está em constante evolução, continue aprendendo e explorando.

- **Não espere demais de seus primeiros relatórios**
  No início, a maioria dos relatórios será marcada como "Não Aplicável" ou "Duplicado." Isso faz parte do processo.
  Aprenda com seus relatórios e atire mais forte na próxima vez.

- **Acredite em si mesmo**
  Confiança e persistência são tão importantes quanto habilidade técnica. Este campo leva uma quantidade enorme de tempo para aprender, mas não é uma habilidade de ficção científica que apenas alguns poucos podem dominar. Se outros conseguiram, você também consegue (apenas certifique-se de ter uma razão forte para começar e que você entenda as dificuldades antes de pular).

## 🤝 Contribuição

Se você tem sugestões, melhorias ou novos recursos para adicionar:

1. Faça um fork deste repositório
2. Faça suas mudanças
3. Envie um Pull Request

Você também pode abrir uma **Issue** 🐛 se encontrar algo que precisa ser corrigido.
