# 🧠 Domain Name System (DNS)

> 🗓️ Data: 01-08-2025

🏷️ **Tags**: #osint #conceitos #rede #network #dns

---

## 📌 Resumo

O Domain Name System (ou DNS) serve para criar uma forma simples para nos comunicarmos com dispositivos na internet sem precisar lembrar números complexos como os IPs. Então, em vez de você lembrar 64.233.185.102 você pode lembrar google.com.

---

## Hierarquia dos Domínios

- ### Top Level Domain (TLD)
  
  É a parte mais a direita do nome de domínio, por exemplo em google.com o `.com` é o TLD. Existem dois tipos de Top Level Domain o gTLD (Generic TLD) e o ccTLD (Country Code TLD). Historicamente os gTLD foram criados com intuito de mostrar para quem estava acessando o proposito do site: `.com` para comercial, `.org` para organizações, `.edu` para educação, `.org` para sites governamentais etc. O ccTLD serve para indicar o local geográfico do site: `.ca` para Canada, `.co.uk` para Reino Unido etc.

- ### Second-Level Domain

  Como no exemplo com o google.com, `.com` é o TLD e o `google` é o Second-Level Domain. Ao registrar um domínio o Second-Level Domain tem um limite de 63 caracteres e utilizar apenas letras, número e hífen (`a-z` `0-9` `-`).

- ### Subdomain

  Os sub domínios são a parte mais a esquerda do domínio, em `translate.google.com` o `translate` é o sub domínio. O nome do sub domínio segue as mesmas limitações do Second-Level Domain: 63 caracteres, letras, números e hífen (`a-z` `0-9` `-`).

## Records

DNS não serve apenas para websites, existem Records para diversas finalidades.

- ### A Record

  Esse Record é para resolver endereços IPv4, ex: 64.233.185.102.

- ### AAAA Record

  Esse Record é para resolver endereços IPv6, ex: 2404:6800:4003:c06::8b

- ### CNAME Record

  Esse Record é para resolver para outros domínios: ex: store.mysite.com resolveria para um CNAME shops.shopify.com.

- ### MX Record

  Esse Record resolve para o servidor que gerencia dos email desse domínio.

- ### TXT Record

  Esse Record é um campo de texto livre onde qualquer texto pode ser armazenado. Ele pode ter várias finalidades, mas as mais comuns incluem: listar nomes de servidores que podem enviar email para o servidor (pode controlar spam e spoofing); verificar a propriedade do domínio quando logar em serviços de terceiros (third-party services).

---

## 🛠️ Ferramentas ou sites relacionados

- [www.nslookup.io](https://www.nslookup.io/) — É uma ferramente online que permite ver DNS Records de sites utilizando seus domínios.
