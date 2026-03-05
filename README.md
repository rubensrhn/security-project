Security Project: Pentest Prático com Kali Linux & Medusa
Este repositório contém a documentação detalhada e os artefatos do desafio prático realizado na plataforma DIO. O objetivo principal é simular ataques de força bruta em ambientes controlados para entender vulnerabilidades e aplicar medidas de mitigação.

🎯 Objetivo do Projeto
Implementar um ambiente de testes de invasão para explorar protocolos comuns (FTP, SMB, HTTP) utilizando a ferramenta Medusa, validando falhas de configuração e senhas fracas em máquinas deliberadamente vulneráveis.

🛠️ Cenário de Laboratório
Para garantir a segurança e o isolamento dos testes, o ambiente foi configurado utilizando virtualização:

Atacante: Kali Linux

Alvos: Metasploitable 2 & DVWA (Damn Vulnerable Web Application)

Rede: Host-Only (Rede Interna) para evitar tráfego externo.

Ferramenta de Ataque: Medusa (Brute-force modular).

🚀 Etapas Executadas
1. Configuração do Ambiente
Instalação das VMs no VirtualBox.

Configuração de adaptadores de rede para comunicação entre as máquinas.

Teste de conectividade via ping e varredura inicial com nmap.

2. Ataques Simulados
Foram realizados três cenários principais de exploração:

Força Bruta em FTP: Tentativas de login automatizadas no serviço de transferência de arquivos.

Automação em Formulário Web (DVWA): Ataque direcionado à interface de login da aplicação web.

Password Spraying em SMB: Enumeração de usuários de rede e teste de senhas comuns para evitar bloqueio de contas.

🛡️ Medidas de Mitigação

Após os testes, foram documentadas as seguintes recomendações:

Políticas de Senhas Fortes: Implementação de complexidade mínima.

Bloqueio de Conta (Account Lockout): Limitar tentativas consecutivas de login.

Desabilitação de Protocolos Inseguros: Substituição de FTP por SFTP/SSH.

2FA (Autenticação de Dois Fatores): Adição de camada extra de segurança em serviços críticos.

⚠️ Aviso Legal (Disclaimer)
Este projeto foi realizado em um ambiente de laboratório controlado para fins estritamente educacionais. Nunca execute ferramentas de varredura ou ataque em redes ou sistemas sem autorização expressa por escrito.

Desenvolvido por [Rubens Norimatsu]
