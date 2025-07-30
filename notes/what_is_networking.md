# 🧠 O que é Networking

> 🗓️ Data: 29-07-2025

🏷️ **Tags**: #osint #conceitos #networking #network

---

## 📌 Resumo

Network (Rede) são coisas simples, como circulo de amigos ou vizinhos conectados por interesses em comum, como hobbies, gostos ou habilidades. Em computação é a mesma coisa, só que em vez de pessoas são dispositivos conectados.

---

## Internet

A internet nada mais é do que uma grande rede global que se conecta com várias outras redes, esse conceito foi criado depois da criação da World Wide Web (WWW) por Tim Berners-Lee em 1989.

- **Redes Privadas**: São as redes menores que se conectam à internet.
- **Redes Pública**: As redes que atuam na intercomunicação entre as rede menores são chamadas de Redes Públicas, ou "A Internet".

## Identificação

Para manter uma ordem os dispositivos precisam ser identificados. Assim como os humanos os dispositivos na internet podem ser identificados com "nomes" e "impressão digital".

- ### IP (Internet Protocol)

  Em resumo os IPs são como uma "impressão digital", eles seguem uma série de regras e só pode existir um por rede, seja ela privada ou pública.

  - **IPv4**: O IPv4 segue um padrão de 4 octetos que vão de 0 à 255. Ex: 192.198.0.1. Isso comporta um total de 2^32 possíveis IPs. (4,29 bilhões).

  - **IPv6**: O IPv6 foi criado para superar essa limitação de combinações do IPv4, nessa versão o IP é formado por 8 partes separadas por dois pontos ":" e comporta um total de 2^128 endereços únicos (mais de 340 trilhões). Ex: 2a00:22c4:a531:c500:425f:cce6:c36b:f64d.

- ### MAC (Media Access Control)

  MAC Address (Media Access Control Address) é um identificador único atribuído à interface de rede de um dispositivo. Ele é composto por 12 caracteres hexadecimais, geralmente exibidos em 6 pares separados por dois-pontos. Ex: a4:c3:f0:85:ac:2d. Os 6 primeiros dígitos (chamados de OUI - Organizationally Unique Identifier) identificam o fabricante da interface de rede, enquanto os 6 últimos são definidos para garantir que cada dispositivo tenha um endereço único. Embora seja projetado para ser único, o MAC Address pode ser facilmente alterado (clonado) em muitos sistemas operacionais. Isso permite que um dispositivo assuma a identidade de outro na rede — uma técnica que pode ser usada, por exemplo, para burlar restrições de acesso baseadas em MAC (como em redes Wi-Fi que usam listas de controle de acesso).

## LAN (Local Area Network)

LAN é uma rede de computadores que conecta dispositivos em uma área geográfica limitada.

- **Switch**: Os Switches são aparelhos dedicados a interligar vários dispositivos (computadores, impressoras etc) via cabo em uma rede de computadores, podendo ter 4, 8, 16, 24, 32 ou até 64 entradas para conexão. Diferentemente de um HUB, o Switch mantém o controle de qual dispositivo está conectado em cada uma das portas, evitando ter que repetir um sinal para todas as entradas e apenas enviando especificamente pro dispositivo certo.

- **Roteador**: Enquanto o Switch conecta aparelhos em uma Network, o Roteador conecta Networks entre si, por um processo chamado Roteamento (dai o nome). Roteamento nada mais é do que o envio de dados entre Redes de Computadores (Networks), esse processo cria um caminho entre elas para que o dado chegue com sucesso no seu destino.

- ### Subnetting

  Subnetting é um termo dado a separação de uma rede em várias sub-redes menores. Por exemplo em uma empresa onde existem diversos setores como Recursos Humanos, Financeiro e Setor de Compras.

  - **Subnet Mask**: A separação em sub-redes ocorre por um número no endereço de IP local que é chamado de Subnet Mask e ele vai de 0 à 255. As sub-redes utilizam o IP de três maneiras diferentes: Identificar a rede, Identificar o Host e Identificar o Gateway padrão. Por exemplo em uma rede onde existe o dispositivo 192.168.[1].100 ele seria um dos Hosts, o 1 seria a identificação da rede e o Gateway poderia ser o primeiro IP ou, geralmente, o ultimo IP da rede 192.168.1.254.
  
    - **Gateway Padrão**: O Gateway padrão é um endereço especial de um dispositivo capaz de enviar dados para fora da rede atual, nesse caso a rede 192.168.1.0.
    - **Host**: Host é qualquer dispositivo da rede que pode enviar e/ou receber dados.
  
## DHCP

Em uma rede de computadores os endereços de IP podem ser atribuídos manualmente em cada dispositivo, ou automaticamente (e mais comum) utilizando DHCP (Dynamic Host Configuration Protocol).

- **Etapas**
  - **DHCP Discover**: Um novo dispositivo chega na rede e se não tiver um IP configurado envia um pedido para ver se a rede possui um DHCP Server.
  - **DHCP Offer**: Caso exista um DHCP Server na rede ele irá responder com um IP para o dispositivo usar.
  - **DHCP Request**: Ao receber o IP para uso o novo dispositivo envia outro pedido para confirmar o uso do IP.
  - **DHCP ACK**: O DHCP Server confirma o uso do IP e o dispositivo pode começar a usar esse endereço.

---

## 🛠️ Ferramentas ou sites relacionados

- [ping](/tools/ping.md)
