# 🧠 ClusterBox

**ClusterBox** é um projeto que transforma TV Boxes com Armbian em um cluster de computação utilizando **OpenPBS**, **NFS** e configuração de rede personalizada.

O objetivo é criar uma alternativa de baixo custo para experimentação, ensino e testes de ambientes de computação distribuída.

---

## 📚 Índice

- [🛠️ Estrutura do Projeto](#️-estrutura-do-projeto)
- [⚙️ Setup do Cluster](#️-setup-do-cluster)
  - [📌 Dependências comuns](#-dependencias-comuns)
  - [📌 Headnode](#-headnode)
  - [📡 Compute Nodes](#-compute-nodes)
  - [📂 NFS Server](#-nfs-server)
- [🌐 Rede e Comunicação](#-rede-e-comunicação)
- [🚀 Envio de Jobs e Uso](#-envio-de-jobs-e-uso)
- [📷 Imagens](#-imagens)
- [📌 Contribuições](#-contribuições)
- [📃 Licença](#-licença)

---

## 🛠️ Estrutura do Projeto

O cluster é composto por:
- 1 Head Node (gerenciador de jobs com OpenPBS)
- 1+ Compute Nodes (execução das tarefas)
- Servidor NFS para compartilhamento de diretórios e sincronização

---

## ⚙️ Setup do Cluster

### 📌 Dependências comuns

Instalação das bibliotecs necessárias e compilação do OpenPBS

👉 [`setup/0-dependencias-comuns.md`](setup/0-dependencias-comuns.md)

### 📌 Headnode

Passo a passo para preparar o **nó principal** com OpenPBS Server + Scheduler + MOM:

👉 [`setup/1-headnode.md`](setup/1-headnode.md)

### 📡 Compute Nodes

Como configurar os nós secundários com OpenPBS MOM:

👉 [`setup/2-compute-nodes.md`](setup/2-compute-nodes.md)

### 📂 NFS Server

Montagem do servidor NFS para sincronização de home e workspace:

👉 [`setup/3-nfs-server.md`](setup/3-nfs-server.md)

---

## 🌐 Rede e Comunicação

Arquivos com:
- Diagrama de rede
- Configuração IP estático ou DHCP
- SSH sem senha
- Resolução de problemas de conexão

👉 [`rede/topologia.md`](rede/topologia.md)  
👉 [`rede/configuracao-ip.md`](rede/configuracao-ip.md)

---

## 🚀 Envio de Jobs e Uso

Como submeter tarefas ao cluster, exemplos de `PBS scripts`, filas, limites e boas práticas:

👉 [`uso/envio-jobs.md`](uso/envio-jobs.md)

---

## 📷 Imagens

Veja diagramas, esquemas de montagem física e prints:

👉 [`/imagens`](imagens/)

---

## 📌 Contribuições

Pull Requests são bem-vindos. Para novas ideias, abra uma issue!

---

## 📃 Licença

Distribuído sob a licença [MIT](LICENSE).

---

> Autor: [Aleqssandro](https://github.com/Aleqssandro)
