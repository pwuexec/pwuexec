---
title: "Do Visual Studio ao Walled Garden A Jornada de um Developer .NET na Era do Open Source"
date: '2025-10-21T09:30:00+01:00'
description: "Durante décadas crescemos dentro do ecossistema Microsoft. Agora percebemos que a liberdade prometida é apenas conveniência disfarçada e que até o open source serve os mesmos donos."
tags: [".NET", "Open Source", "Azure", "Linux", "Carreira"]
draft: false
cover:
  image: "/images/posts/dotnet-walled-garden/cover.png"
  alt: "Um developer .NET a tentar sair do Walled Garden da Microsoft"
  relative: false
---

Durante décadas crescemos dentro do ecossistema Microsoft. Agora percebemos que a liberdade prometida é apenas conveniência disfarçada e que até o open source serve os mesmos donos.

# Do Visual Studio ao Walled Garden A Jornada de um Developer .NET na Era do Open Source

## A Perspetiva de um Developer .NET Crescido no Mundo Microsoft

Durante décadas o mundo do desenvolvimento europeu cresceu sob a mesma bandeira. Escolas, universidades e centros de formação ensinaram programação em ambientes Windows. Servidores públicos e sistemas governamentais foram construídos em cima do stack Microsoft. E as empresas seguiram o mesmo caminho porque era a opção mais natural e aparentemente segura.  
Para muitos de nós a história começou no Visual Studio. O primeiro "Hello World" correu num Windows XP e a primeira aplicação de produção foi publicada num IIS dentro da rede da empresa. Este percurso não foi exceção, foi a norma. O ecossistema Microsoft criou as condições perfeitas para nos manter ali. A formação estava alinhada, o mercado pedia essas competências e a curva de entrada era suave.  
Com a chegada do fim do Windows 10 algo começou a mudar. Governos e organizações públicas europeias começaram a repensar a dependência de soluções proprietárias. Iniciativas como **goeuropean** e **european-alternatives** nasceram precisamente com esse objetivo: reduzir a dependência tecnológica de fornecedores únicos e apostar em soluções open source. De repente a conversa sobre liberdade deixou de ser teórica e passou a ser estratégica.  

## O Conforto da Prisão Dourada

Para quem sempre viveu dentro do ecossistema Microsoft tudo parecia natural. Visual Studio funcionava sem esforço e a produtividade era quase instantânea. IIS e Windows Server eram sinónimos de estabilidade e o ciclo de desenvolvimento era tão fluido que mal nos apercebíamos da prisão em que estávamos.  
O preço dessa conveniência era invisível. O código não respirava fora daquele casulo e cada passo fora do ambiente oficial parecia uma aventura perigosa. Dependíamos de ferramentas proprietárias, de licenças caras e de uma forma de pensar que se confundia com a própria plataforma.  
A Microsoft construiu um império à custa desta dependência. Criou ferramentas tão integradas e polidas que a ideia de procurar alternativas parecia desnecessária. E muitos de nós aceitaram esse contrato sem questionar.  

## O Circo do Windows e a Ditadura dos Clicks

O Windows sempre foi a porta de entrada para o mundo Microsoft e também a sua armadilha mais eficaz. A experiência inicial é sedutora. Dois cliques e o projeto está a correr. O sistema trata de tudo por nós e o ambiente parece feito à medida do developer. Mas essa conveniência tem um preço elevado.  
As decisões controversas acumulam-se  

1. As contas locais desapareceram. Agora é obrigatório usar uma conta Microsoft para iniciar sessão.  
2. O consumo de RAM disparou. Uma instalação limpa consome vários gigabytes sem correr nada de relevante.  
3. As atualizações obrigatórias transformam a produtividade em sorte. Um reboot inesperado no meio de um deployment deixou de ser acidente e passou a ser feature.  
4. O Game Pass aumentou de preço e é apresentado como benefício.  

Estes problemas são apenas a ponta do iceberg. O Windows está carregado de telemetria que recolhe dados de forma constante e muitas vezes invisível. Mesmo com todas as opções de privacidade desativadas há serviços que continuam a comunicar em segundo plano.  
O sistema vem cheio de aplicações pré-instaladas que ninguém pediu. Widgets, promoções e software redundante ocupam espaço e consomem recursos. Em muitas empresas o primeiro passo após a instalação é limpar o sistema antes de começar a trabalhar.  
A interface é um caos. Configurações estão divididas entre a aplicação moderna e o velho Painel de Controlo. Tarefas simples exigem múltiplos cliques e menus escondidos. A coerência deu lugar a um UX que parece feito para confundir.  
E mesmo quando tentamos exercer escolha, o sistema impõe-se. O Microsoft Edge abre links internos mesmo quando outro browser está definido por defeito. Não é preferência, é imposição.  
A versão 25H2 do Windows 11 empurrou a situação para o absurdo. O localhost passou a comportar-se de forma errática e o desenvolvimento local deixou de ser fiável.  
E quanto ao velho companheiro Windows 10? Esse já foi oficialmente abandonado. A Microsoft não o matou de um dia para o outro, escolheu a crueldade lenta. Deixou-o a definhar no canto enquanto anuncia que, a partir de agora, a segurança tem mensalidade. Se quiseres continuar a usá-lo em produção depois do fim do suporte em outubro de 2025, prepara a carteira. O que antes era um sistema operativo de trabalho transformou-se num produto por subscrição, e a mensagem é clara: ou migras para o Windows 11 ou pagas para continuar a ter atualizações.  

## O Teatrinho do Open Source

Durante muito tempo a Microsoft tratou o open source com desdém. Steve Ballmer chegou a chamar ao Linux um cancro. Depois o mercado mudou e o discurso mudou com ele. Hoje a empresa proclama amor ao open source mas as ações contam outra história.  
A comunidade criou ferramentas essenciais para o ecossistema .NET. Containers de injeção de dependências, frameworks de UI e soluções de messaging nasceram do esforço coletivo. Em vez de apoiar esses projetos a Microsoft decidiu reescrevê-los.  

- O Autofac era um container maduro e amplamente usado. A empresa criou o seu próprio.  
- Uno Platform e Avalonia eram soluções UI sólidas. A empresa lançou o .NET MAUI e promoveu-o como padrão.  

O resultado é que muitos projetos comunitários começaram a mudar de licença. MassTransit, FluentAssertions e MediatR adotaram modelos comerciais não por ganância mas porque foram explorados durante anos por gigantes sem retorno.  

## O Walled Garden Azul

O conceito de Walled Garden descreve perfeitamente a abordagem moderna da Microsoft. Tudo funciona com uma fluidez impressionante desde que se permaneça dentro das muralhas. Visual Studio integra-se automaticamente com o Azure DevOps. Ferramentas como Key Vault ou Service Bus exigem zero configuração.  
Mas essa comodidade cria dependência. Aplicações que usam serviços Azure tornam-se difíceis de migrar. O processo não é uma simples mudança de fornecedor. É uma reescrita estrutural que pode levar meses e exigir uma equipa inteira.  
A realidade é que .NET funciona em **self-host**, **AWS** ou **GCP**. No entanto, a documentação oficial, os exemplos e a interface das ferramentas guiam-nos consistentemente para o Azure. É um empurrão subtil mas constante.  

## A Grande Fuga para o Mundo Livre

Perante tudo isto muitos developers decidiram saltar a cerca. A escolha natural foi o Linux. E entre as várias opções, Arch Linux surgiu como o símbolo máximo de controlo e liberdade.  
A mudança foi libertadora e dolorosa ao mesmo tempo. Sem a conveniência do ecossistema Microsoft tudo passou a exigir mais atenção. Configurar ambientes deixou de ser automático e passou a ser artesanal. Debuggers que funcionavam com um clique pediam agora ajustes manuais.  
O que antes era plug and play tornou-se uma sequência de decisões e configurações conscientes. Nada acontecia sozinho. A liberdade existia mas obrigava-nos a assumir responsabilidades que tínhamos esquecido.  
Esta experiência revelou a verdade incómoda. O que a Microsoft oferece não é apenas tecnologia. É dependência embrulhada em conforto.  

## A Liberdade com Rodinhas

Não há dúvida de que .NET é uma plataforma tecnicamente poderosa. C# é elegante, a performance é de topo e a comunidade é vibrante. Mas toda essa excelência vem acompanhada de condições.  
A liberdade de escolha existe no papel mas está cercada pela conveniência. Enquanto aceitarmos as regras do Walled Garden tudo funciona perfeitamente. Quando decidimos sair, descobrimos o preço da independência.  
O open source que a Microsoft defende tem a profundidade de uma estratégia de marketing. O código pode estar disponível mas a estrutura que o rodeia continua a servir os interesses da empresa.  

## Conclusão A Prisão Confortável

O ecossistema Microsoft permanece um dos mais poderosos do mundo do desenvolvimento. Mas também continua a ser um dos mais controladores. O Walled Garden é confortável e eficiente mas é também um lembrete de que cada escolha tem um custo.  
A empresa aprendeu que abrir o código era vantajoso para o negócio. Não no espírito do open source mas como forma de atrair developers e manter a dependência através da infraestrutura.  
O abandono do Windows 10 é o exemplo perfeito dessa estratégia. Em vez de manter uma base estável e acessível, a Microsoft escolheu empurrar milhões de utilizadores para o Windows 11. Não o fez por necessidade técnica, fez porque é assim que se vende o próximo produto. É obsolescência planeada com verniz corporativo e o recado é simples: quem quiser segurança vai ter de pagar.  
Podemos correr .NET em qualquer lado. Podemos evitar o Azure. Podemos construir soluções totalmente independentes. Mas a experiência oficial guia-nos sempre na mesma direção.  
Chama-lhe liberdade se quiseres. Para muitos de nós é liberdade com rodinhas. Confortável e previsível mas com a Microsoft a segurar o guiador. E enquanto aceitarmos isso o ar continuará a ser pago e o código continuará a ter dono.

---
