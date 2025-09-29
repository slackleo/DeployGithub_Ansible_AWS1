# Projeto: Congelamento e Backup de Banco de Dados

## Objetivo
Criar um processo seguro e consistente para congelamento e backup de bancos de dados em AWS, garantindo integridade e automação.

## Cenário
Demanda de freelance para criar snapshot consistente em RDS, DynamoDB e EC2, seguindo boas práticas de segurança.

## Tecnologias usadas
- AWS CLI
- Terraform
- Ansible
- GitHub Actions (pipeline)
- Bash Scripts

## Arquitetura
![Diagrama](./imagens/diagrama.png)

## Passo a passo
Veja [docs/passo_a_passo.md](./docs/passo_a_passo.md).

## Scripts
- `backup_rds.sh`: script para snapshot manual em RDS.
- `backup_ec2.sh`: script para snapshot EBS com lock.
- `playbook_ansible.yml`: automatização do processo.

## Boas práticas
- Uso de IAM Roles com princípio do menor privilégio.
- MFA para acesso.
- Automatização via pipeline CI/CD.

## Resultados
- Processo seguro e repetível.
- Redução de tempo para execução: 35 minutos.
- Documentação clara para replicação.

## Documentação extra
- [Políticas IAM](./docs/politicas_iam.md)
