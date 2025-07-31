# 🧠 Firewall

> 🗓️ Data: 31-07-2025

🏷️ **Tags**: #osint #ferramentas #conceitos #segurança #rede #network #firewall

---

## 📌 Resumo

É um dispositivo na rede responsável por permitir ou negar entrada e/ou saída de tráfego com base em regras definidas.

---

## Responsabilidades do Firewall

- **Entrada de dados**: De onde o tráfego está vindo? O Firewall foi configurado para aceitar ou recusar essa origem?
- **Saída de dados**: Para onde o tráfego está indo? O Firewall foi configurado para aceitar ou recusar esse destino?
- **Controle de Portas**: Para qual porta o tráfego vai? O Firewall foi configurado para aceitar ou recusar tráfego nessa porta?
  - **Portas**: São identificadores que auxiliam comunicações entre diferentes dispositivos e aplicações. Existem alguns standards para determinadas portas, como por exemplo a porta 80 para aplicações HTTP ou 443 para aplicações HTTPS.
- **Controle de Protocolos**: Qual o protocolo do tráfego? O Firewall foi configurado para aceitar ou recusar TCP, UDP ou ambos?

## Tipos de Firewall

- ### Stateful

Stateful é um tipo de firewall que usa toda a informação de uma conexão, em vez de pacotes individuais, para tomada de decisão. Ele consume bem mais recursos por fazer decisões dinamicamente.

- ### Stateless

Stateless é um tipo de firewall que usa um conjunto de regras estáticas para tomada de decisão. Ele usa muito menos recursos, mas por esse motivo, sua eficacia depende totalmente do conjunto de regras ser bem configurado.
