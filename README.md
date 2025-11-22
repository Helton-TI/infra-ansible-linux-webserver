# Automação de Servidor Linux com Ansible e Tomcat

Este repositório contém um laboratório de automação de infraestrutura utilizando **Ansible** para configurar um servidor Linux com:

- Pacotes básicos de administração
- Instalação do Java
- Instalação e configuração do **Apache Tomcat**
- Estrutura organizada com **playbooks**, **roles**, **inventário** e **ansible.cfg**

> Objetivo: demonstrar conhecimentos práticos em Administração de Sistemas Linux, Ansible, Shell Script e servidores de aplicações (Tomcat), alinhado a ambientes críticos e de produção.

---

## 🧩 Arquitetura do Lab

- **Sistema operativo alvo**: Linux (Ubuntu Server / Debian)
- **Control node**: máquina com Ansible instalado
- **Serviço configurado**: Apache Tomcat

---

## 📂 Estrutura do projeto (planeada)

```text
infra-ansible-linux-webserver/
├─ ansible.cfg
├─ inventory
├─ playbooks/
│  └─ site.yml
└─ roles/
   ├─ common/
   │  └─ tasks/main.yml
   └─ tomcat/
      ├─ tasks/main.yml
      └─ templates/server.xml.j2

