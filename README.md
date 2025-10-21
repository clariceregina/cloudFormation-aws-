# 📘 AWS CloudFormation - Visão Geral

## 🔧 O que é o AWS CloudFormation?

O **AWS CloudFormation** é um serviço da Amazon Web Services que permite provisionar e gerenciar recursos de nuvem usando **infraestrutura como código (IaC)**. Com ele, é possível criar, atualizar e deletar toda a infraestrutura de forma automatizada e reproduzível, por meio de arquivos de modelo (*templates*).

---

## 📄 Formatos de Modelos (Templates)

Os modelos do CloudFormation podem ser escritos em dois formatos principais:

1. **YAML** (`.yaml` ou `.yml`)
2. **JSON** (`.json`)

## 🏗️ Como criar uma Stack

Uma **Stack** é uma instância de um modelo (template) sendo executada, ou seja, é a representação dos recursos criados no ambiente AWS.

### Métodos para criar uma stack:

#### 1. Via Console AWS

#### 2. Via AWS CLI

#### 3. Via AWS SDKs (Python - Boto3)

## ⚖️ CloudFormation vs Terraform

| Característica             | **AWS CloudFormation**                            | **Terraform (HashiCorp)**                            |
|----------------------------|---------------------------------------------------|------------------------------------------------------|
| **Escopo**                 | Exclusivo para recursos AWS                      | Multi-cloud (AWS, Azure, GCP, etc.)                  |
| **Linguagem**              | YAML ou JSON                                     | HCL (HashiCorp Configuration Language)               |
| **Arquivo de estado (state)** | Gerenciado automaticamente pela AWS              | Requer gerenciamento manual (state file)             |
| **Modularidade**           | Suporte via *nested stacks*                      | Suporte mais avançado com módulos reutilizáveis      |
| **Gerenciamento**          | Integrado diretamente com a AWS                  | Independente, com backend configurável               |
| **Ferramentas disponíveis**| AWS Console, AWS CLI, SDKs                       | Terraform CLI                                        |
| **Curva de aprendizado**   | Mais simples para quem já usa AWS                | Mais complexa, mas com maior flexibilidade           |

---

## ✅ Quando usar qual?

- ✅ Use **CloudFormation** se:
  - Seu ambiente for **100% AWS**
  - Você deseja integração nativa com os serviços da AWS
  - Prefere não gerenciar arquivos de estado manualmente

- 🌐 Use **Terraform** se:
  - Você trabalha com **múltiplos provedores de nuvem**
  - Deseja **mais controle sobre o ciclo de vida** dos recursos
  - Precisa de **reutilização avançada** com módulos e melhor controle de dependências
