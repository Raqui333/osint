# 🧠 Virtual Private Network (VPN)

> 🗓️ Data: 31-07-2025

🏷️ **Tags**: #osint #ferramentas #conceitos #segurança #rede #network #vpn

---

## 📌 Resumo

Virtual Private Network (ou VPN) é uma tecnologia que permite criar um caminho especifico (túnel) na internet para conexão entre dois dispositivos. Dispositivos nesse túnel formam sua própria rede privada virtual.

---

## Benefícios

- ### Privacidade

  A tecnologia VPN utiliza criptografia para proteção de dados. Isso significa que os dados só podem ser entendidos por quem envia e por quem recebe. Essa criptografia pode ser útil em WiFi públicos, onde a rede não oferece nenhuma proteção aos dados. Você pode usar uma VPN para proteger seus dados de serem vistos por outra pessoa.

- ### Anonimato

  Em países onde a liberdade de expressão é controlada, seu tráfego pode ser vistos e localizado por seu provedor de internet (ISP) ou por outros intermediadores. O uso de VPN nesses casos pode te proteger.
  > O nível de anonimato na VPN vai depender também dos outros dispositivos respeitarem essa privacidade, utilizar VPNs que capturam logs e/ou armazenam histórico é o mesmo que não usar.

## Tecnologias

- ### PPP

  Essa tecnologia é usado pelo PPTP para permitir autenticação e garantir a criptografia dos dados. VPNs funcionam utilizando uma chave privada e um certificado público, ambos precisam corresponder para a conexão funcionar.
  > Não cria por si só uma rede.

- ### PPTP

  Point-to-Point Tunneling Protocol (PPTP) é a tecnologia que permite dados PPP navegarem pela rede. Apesar de facilmente configurável ele tem uma criptografia mais fraco em comparação com outras alternativas.

- ### IPSec

  Internet Protocol Security (IPSec) criptografa os dados usando o já existente Internet Protocol (IP) framework. É mais difícil de configurar, porém permite uma forte criptografia de dados e é suportados em muitos dispositivos.
