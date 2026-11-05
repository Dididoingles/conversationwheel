# Conversation wheel

Uma aplicação web estática para prática de conversação em inglês, organizada em três níveis de proficiência. O usuário gira uma roleta que sorteia um tópico de conversa e, em seguida, utiliza um cronômetro de um minuto para desenvolver a resposta em voz alta.

O projeto foi pensado para uso em sala de aula ou estudo individual, com uma interface discreta, tipografia consistente e feedback sonoro e visual em cada etapa.

Acesse através do link: https://dididoingles.github.io/conversationwheel/

## Sumário

- [Visão geral](#visão-geral)
- [Estrutura do projeto](#estrutura-do-projeto)
- [Níveis disponíveis](#níveis-disponíveis)
- [Como usar](#como-usar)
- [Funcionalidades](#funcionalidades)
- [Tecnologias](#tecnologias)
- [Áudio](#áudio)
- [Página 404](#página-404)
- [Execução local](#execução-local)
- [Licença](#licença)

## Visão geral

O Conversation Spinner é composto por três telas principais:

1. **Seleção de nível** — o usuário escolhe entre Easy, Intermediate e Advanced.
2. **Roleta da conversa** — cada nível possui sua própria roleta com trinta perguntas calibradas para o estágio correspondente.
3. **Overlay de conclusão** — ao encerrar o tempo, uma mensagem de conclusão é exibida com animação e opção de continuar.

O design evita containers fechados e se apoia em tipografia, espaçamento e gradientes sutis para construir hierarquia visual. A identidade é mantida em todas as telas: mesma paleta escura, mesma família tipográfica e o mesmo padrão de animações.

## Estrutura do projeto
.
├── index.html Página inicial com seleção de níveis
├── 404.html Página de erro personalizada
├── gm.ico Favicon
├── easy/
│ └── index.html Roleta nível Easy (A1–A2)
├── intermediate/
│ └── index.html Roleta nível Intermediate (B1–B2)
└── advanced/
└── index.html Roleta nível Advanced (C1–C2)

text

## Níveis disponíveis

Cada nível possui trinta perguntas próprias, com complexidade crescente de estrutura e vocabulário.

**Easy (A1–A2)**
Perguntas diretas sobre rotina, preferências, família, hobbies e memórias simples. As respostas esperadas são curtas e descritivas.

**Intermediate (B1–B2)**
Perguntas que exigem opinião, justificativa, comparação e narrativa. Incluem condicionais, prós e contras e experiências pessoais.

**Advanced (C1–C2)**
Perguntas abstratas que demandam argumentação estruturada, avaliação crítica e hipóteses complexas. O vocabulário e as estruturas são sofisticados.

## Como usar

1. Abra a página inicial e escolha um nível.
2. Clique em "Girar a roleta" ou pressione a barra de espaço.
3. Aguarde o sorteio. A pergunta aparece junto com o cronômetro.
4. Clique em "Iniciar" para começar a contagem de um minuto.
5. Ao final do tempo, ou ao clicar em "Encerrar", a overlay de conclusão é exibida.
6. Clique em "Continuar" para voltar à roleta.

A roleta não repete perguntas até que todas as trinta tenham sido sorteadas. Ao final de um ciclo, o baralho é embaralhado novamente e as fatias voltam a ficar visíveis.

## Funcionalidades

- Roleta com sorteio sem repetição dentro do ciclo.
- Cronômetro circular de um minuto com pausa, reinício e encerramento manual.
- Overlay de conclusão com animação de verificação desenhada em SVG.
- Feedback sonoro em todas as ações relevantes.
- Layout responsivo com comportamentos distintos para desktop e mobile.
- Atalho de barra de espaço para girar a roleta.
- Fechamento da overlay com a tecla Escape.
- Página 404 personalizada com roleta animada.

## Tecnologias

O projeto é inteiramente estático e não requer build, dependências ou servidor de aplicação.

- HTML5
- CSS3 (variáveis, grid, flexbox, animações)
- JavaScript puro, sem frameworks
- SVG para a roleta, o cronômetro e os ícones
- Google Fonts para a família Poppins

Não há backend, banco de dados ou processo de autenticação. Toda a lógica é executada no navegador do usuário.

## Áudio

Os arquivos de áudio são hospedados externamente e referenciados por URL. Os sons utilizados são:

- Som da roleta girando, tocado durante o sorteio.
- Som de clique, utilizado nos botões e nos eventos do cronômetro.
- Alertas de fim de tempo, derivados do som de clique com variação de tom.

As URLs estão declaradas no início do bloco de script de cada página. Caso os arquivos sejam movidos ou substituídos, basta atualizar essas referências.

##Licença
Este projeto é disponibilizado gratuitamente para uso pessoal e educacional.

A venda, redistribuição comercial, reprodução integral em outros projetos ou publicação como produto próprio não são permitidas.

O uso é livre para professores, estudantes e qualquer pessoa que deseje praticar conversação em inglês. Modificações para uso próprio são permitidas, desde que o projeto resultante não seja comercializado.

Para usos que não se enquadrem nessas condições, entre em contato pelo perfil indicado no rodapé da aplicação.
