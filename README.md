<h1 align="center">Kit de Desenvolvimento do Ladesa</h1>

<p align="center">Recursos feitos para o ambiente local de desenvolvimento dos serviços 💝.</p>

<p align="center">
 <a href="https://github.com/ladesa-ro/dev-kit/blob/main/LICENSE" target="_blank"><img alt="📝 License: MIT" src="https://img.shields.io/badge/%F0%9F%93%9D_license-MIT-21bb42.svg"></a>
</p>

<img align="right" alt="Project logo: the TypeScript blue square with rounded corners, but a plus sign instead of 'TS'" src="https://avatars.githubusercontent.com/u/143351320?s=128&v=4" height="128">

O _Kit de Desenvolvimento do Ladesa_ fornece aos colaboradores o guia e passo-a-passo para a configuração de desenvolvimento para qualquer um que queira contribuir com o Ladesa.

## Vamos Começar

### Configurar um Emulador de Terminal

- <https://docs.ladesa.com.br/developers/tutorials/os/command-line/>

### Configurar o Git

- [Git](https://git-scm.com/downloads)
- <https://docs.ladesa.com.br/developers/tutorials/source-code/git/>

### Configurar o Docker

- [Docker Engine](https://docs.docker.com/engine/install/)
- <https://docs.ladesa.com.br/developers/tutorials/platforms/containers/docker/>

## Recursos do Kit de Desenvolvimento do Ladesa

### Obter o ladesa-ro/dev-kit

```sh
git clone https://github.com/ladesa-ro/dev-kit.git
cd dev-kit
```

### Proxy Reverso

```sh
cd reverse-proxy
```

```sh
make up
```

Acesso ao dashboard do Traefik em: <http://traefik.ladesa.localhost>.

### Message Broker RabbitMQ

```sh
cd message-broker
```

```sh
make up
```

Acesso ao dashboard do RabbitMQ em: <http://mq.ladesa.localhost>.

## Licença

[MIT](./LICENSE) © 2022 – presente, Ladesa.
