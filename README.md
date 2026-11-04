# ☁️ Projeto: criando uma arquitetura resiliente / Semana de Arquitetura AWS]

Documentação da arquitetura e dos laboratórios práticos realizados com foco na certificação **AWS Certified Solutions Architect – Associate**.

---

## 🎯 Sobre o Projeto
Breve descrição do que este laboratório resolve ou demonstra. Exemplo: *Implementação de uma aplicação web altamente disponível, escalável e tolerante a falhas utilizando serviços gerenciados da AWS.*

---

## 🏗️ Arquitetura da Solução
Explique de forma visual ou textual como os componentes da AWS se comunicam.

*(Opcional: Insira uma imagem da arquitetura desenhada ou gerada)*
> ![Diagrama de Arquitetura](./diagrams/arquitetura.png)

### Principais Componentes Utilizados:
* **Amazon VPC:** Isolamento de rede, divisão em Subnets públicas e privadas (Multi-AZ).
* **Application Load Balancer (ALB):** Distribuição de tráfego HTTP/HTTPS entre instâncias EC2.
* **Amazon EC2:** Hospedagem da camada de aplicação em instâncias escaláveis.
* **Amazon RDS:** Camada de banco de dados relacional gerenciado em alta disponibilidade.
* **AWS IAM:** Gerenciamento seguro de identidades, papéis (Roles) e permissões de acesso.

---

## 🚀 Como Executar / Replicar o Laboratório
Passo a passo básico de como o ambiente foi configurado:

1. **Configuração de Rede (VPC):**
   * Criação de uma VPC com blocos CIDR customizados.
   * Configuração de tabelas de rotas e Internet Gateway.
2. **Provisionamento de Bancos de Dados:**
   * Lançamento de uma instância Amazon RDS em sub-redes privadas.
3. **Implantação de Instâncias e Balanceamento:**
   * Criação do Auto Scaling Group associado ao Application Load Balancer.

---

## 💡 Aprendizados e Boas Práticas (Well-Architected Framework)
* **Segurança:** Uso do princípio de privilégio mínimo no IAM e isolamento de banco de dados na rede privada.
* **Confiabilidade:** Utilização de múltiplas zonas de disponibilidade (Multi-AZ) para evitar pontos únicos de falha (SPOF).
* **Performance:** Aplicação de balanceamento de carga para otimizar a distribuição de requisições.

---

## 🛠️ Tecnologias e Ferramentas
* **Cloud Provider:** Amazon Web Services (AWS)
* **Ferramentas:** AWS Management Console, Git, GitHub.
