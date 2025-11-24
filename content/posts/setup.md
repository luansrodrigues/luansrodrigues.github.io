---
title: "Por que criei este blog: minha jornada em cibersegurança, meu laboratório e meu processo de aprendizagem"
date: 2025-11-23
draft: false
categories:
  - "Cybersecurity"
  - "Forensics"
  - "Linux"
  - "Learning"
tags:
  - "ThinkPad"
  - "Fedora"
  - "Hardening"
  - "TryHackMe"
  - "HackTheBox"
  - "CTF"
  - "OSINT"
  - "Linux Security"
  - "Forense Digital"
description: "Como desenvolvedor frontend e estudante de Pós-Graduação em Cibersegurança, montei meu próprio laboratório com um ThinkPad X230 e Fedora. Documentar meu aprendizado em hardening, forense, redes e plataformas como TryHackMe e HTB virou parte essencial da minha formação."
keywords:
  - "estudante de cibersegurança"
  - "jornada na cibersegurança"
  - "tryhackme"
  - "hack the box"
  - "ctf hardening"
  - "thinkpad x230"
  - "fedora security"
  - "linux hardening"
  - "osint"
  - "laboratório de segurança"
image: "/images/posts/jornada-cyber.png"
level: "Intermediário"
---


Sou desenvolvedor **frontend**. Meu dia a dia sempre foi JavaScript, componentes, UI, experiência do usuário. Mas, em algum momento, percebi que havia um lado meu que queria ir além da superfície — queria entender sistemas de verdade, redes de verdade, segurança de verdade.

E descobri que a única forma de aprender isso era **estudar por conta própria**. Foi assim que cibersegurança deixou de ser só uma curiosidade e virou meu **hobby sério** — aquele assunto que estudo à noite, nos fins de semana, nos momentos livres. Não porque o trabalho exige, mas porque eu genuinamente gosto de mergulhar fundo.

Eu criei este blog porque percebi que **documentar meu aprendizado é tão importante quanto estudar**. Quando algo quebra e eu conserto, escrevo. Quando aprendo algo novo, escrevo. Quando erro de novo, escrevo também.

Este blog virou meu caderno digital — e o reflexo da minha própria evolução.

### Meu Laboratório de Estudos

Como dev frontend, eu sempre vivi na camada mais alta da tecnologia: navegador, APIs, UI, frameworks. Mas quando entrei no mundo de segurança, percebi que queria justamente o contrário: **entender o que está embaixo**.

Então montei meu próprio laboratório. Sem regras. Sem medo de apagar algo. Sem medo de quebrar.

Um lugar para:

* entender kernel, memória, processos e permissões
* testar vulnerabilidades sem medo
* estudar hardening e ver consequências reais
* analisar tráfego e protocolos de verdade
* praticar forense digital
* aprender fazendo e errando

Foi o melhor investimento que fiz na minha formação.

### Meu Setup: ThinkPad X230 + Fedora Linux

{{< case title="Meu Setup Principal" impact="Laboratório de estudos pessoal" date="2024" >}}
ThinkPad X230 rodando Fedora Linux — minha estação de trabalho e laboratório de estudos em um só dispositivo.
{{< /case >}}

### Por que escolhi o ThinkPad X230?

Eu precisava de uma máquina que não tivesse medo de abrir, desmontar, resetar e arriscar. Como desenvolvedor frontend, meu computador principal não podia ser meu laboratório de erros. O X230 virou esse espaço livre.

**Vantagens para alguém como eu — dev de dia, estudante de segurança à noite:**

* fácil de desmontar
* modular
* compatível com praticamente qualquer distro Linux
* resistente
* perfeito para estudar hardware e firmware

O X230 não é só um notebook velho. Ele virou *meu laboratório físico*.

### Por que Fedora? Por que não Kali ou Parrot?

Como alguém vindo do mundo de frontend, eu nunca quis um sistema que me desse tudo pronto. Eu queria construir meu entendimento com as próprias mãos.

Por isso escolhi Fedora: eu queria sentir a estrutura real de um sistema Linux moderno. Queria trabalhar com SELinux, systemd, journald, política, initramfs, módulos — coisas que jamais aparecem no meu trabalho formal, mas que eram exatamente o que eu buscava aprender.

Fedora me obriga a:

* entender o SELinux a fundo
* trabalhar com systemd e suas units
* ajustar journald para auditoria
* configurar firewall manualmente
* instalar ferramentas sem presets
* lidar com kernel moderno e patches recentes

É mais difícil? Sim. Mas também é o que me faz aprender de verdade.

Quando algo quebra, eu sei que fui eu quem quebrou. E isso é libertador.

## Criptografia de Disco: Onde Aprendi Que Segurança Tem Custo

Quando configurei LUKS2 com Argon2id, achei que estava “fazendo tudo certo”. Até perceber que o boot estava levando **4 minutos** só para derivar a chave.

A solução veio com estudo, teste, benchmark e ajustes.

Hoje entendo:

* o que é uma função memory-hard
* como funciona a derivação da chave
* quando trocar velocidade por segurança
* quando isso é exagero

E principalmente:

> segurança sem equilíbrio vira dor de cabeça.

## Hardening: Meu Aprendizado Mais Profundo

Como dev frontend, eu nunca tinha precisado pensar em `/etc/fstab`, mount flags, initramfs ou permissões de kernel. Mas quando comecei hardening no meu laboratório, foi inevitável.

Aprendi:

* como ASLR funciona na prática
* como o kernel aplica Lockdown Mode
* por que `noexec` em `/tmp` bloqueia muita coisa
* que SELinux não é um inimigo — é um professor

Passei dias quebrando ferramentas, restaurando permissões, lendo logs enigmáticos como:

```
avc: denied { read write } for pid=1337 comm="python" ...
```

E cada linha dessas me ensinou mais do que um curso inteiro.

## Aprendendo Redes e Wi-Fi: Meu Ponto de Virada

A primeira vez que capturei tráfego real com `tcpdump`, percebi o abismo entre teoria e prática.

Passei semanas:

* analisando handshakes WPA2
* capturando beacon frames
* estudando tráfego em modo monitor
* entendendo 802.11 frame por frame
* usando `airodump-ng`, `kismet`, `bettercap`

E isso mudou completamente minha visão sobre redes.

## TryHackMe, Hack The Box e CTFs: Meu Ciclo de Aprendizado

Meu ciclo é simples:
**estudo → reproduzo no lab → aplico em CTF → documento**

TryHackMe me deu a base.
Hack The Box me ensinou humildade.
CTFs me ensinaram metodologia.

Hoje minha rotina é:

* trabalhar com frontend
* estudar segurança à noite
* fazer labs aos poucos
* documentar tudo no blog

Essa disciplina mudou minha relação com tecnologia.

## Pós-Graduação: Conectando a Teoria à Prática

Mesmo trabalhando como dev frontend, eu decidi dar um passo além e formalizar meus estudos com uma **Pós-Graduação em Cibersegurança**. Foi uma escolha pessoal, não profissional: eu queria entender segurança com profundidade acadêmica, mesmo que isso não tivesse ligação direta com meu dia a dia no trabalho.

Minha vida hoje é assim:

* trabalho com frontend durante o dia,
* estudo segurança à noite,
* e, quando sobra tempo, mergulho no meu laboratório para praticar.

Esses mundos não competem — eles se complementam.

## Epílogo: O Que Eu Gostaria De Ter Sabido Antes

Se eu pudesse falar com o Luan que estava começando, eu diria:

* você vai quebrar tudo, e isso é parte do processo
* leia logs antes de reinstalar
* estude o porquê, não só o como
* documente para lembrar
* permita-se ser curioso
* sua profissão não define seus limites técnicos

Eu não escolhi segurança como carreira. Eu escolhi segurança como caminho de aprendizado.

E isso foi o que mais me transformou.

## Guia Para Iniciantes (Versão Mentor)

* Você vai errar. E isso é bom.
* Escolha uma máquina que você não tenha medo de quebrar.
* Trate o Linux como um organismo real.
* Aprenda a depurar antes de reinstalar.
* Hardening não é copiar comandos da internet.
* SELinux está tentando te ajudar.
* Entenda o boot.
* Evite exageros em criptografia.
* Comece ROP cedo.
* Em CTFs, versão importa.
* Documente tudo.
* Não tenha pressa.
