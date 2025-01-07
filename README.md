# Documentação do Azure - Serviços para Desenvolvimento e Gerenciamento
Este README descreve os principais serviços do Microsoft Azure relacionados ao desenvolvimento de aplicações, gerenciamento de APIs, segurança, armazenamento e outros tópicos abordados na Certificação AZ-204: Desenvolvedor do Microsoft Azure.

## **Índice**
1. [📖Introdução](#introdução)
2. [Gerenciamento de API](#gerenciamento-de-api)
3. [Segurança e Gestão de Segredos](#segurança-e-gestão=de=segredos)
4. [Armazenamento](#armazenamento)
5. [Configuração Centralizada](#configuração-centralizada)
6. [Mensageria e Filas](#mensageria-e-filas)
7. [Monitoramento e Diagnóstico](#monitoramento-ediagnóstico)
8. [Desenvolvimento e Implementação](#desenvolvimento-e-implementação)
9. [Recursos Adicionais](#recursos-adicionais)

## Introdução
O Microsoft Azure oferece uma ampla gama de serviços para desenvolvedores que buscam criar, implementar e gerenciar aplicativos escaláveis, seguros e resilientes. Este documento cobre os serviços mais usados e suas funcionalidades principais, ajudando você a entender seu propósito e uso em projetos reais.

## Gerenciamento de API 
O Azure API Management ajuda no gerenciamento de APIs internas e externas, oferecendo recursos como:

- Controle de acesso: Autenticação baseada em certificados, tokens e chaves de API.
- Políticas configuráveis: Aplicação de limites de taxa (rate limiting), transformação de payloads e manipulação de cabeçalhos.
- Publicação simplificada: Criação de portais para desenvolvedores, incluindo documentação e chaves de acesso.
**Exemplo de caso de uso:**
Controlar o número de chamadas à API para evitar sobrecarga, garantindo acesso apenas a clientes autenticados.

## Segurança e Gestão de Segredos 
O Azure Key Vault é essencial para proteger informações sensíveis, como:

- Segredos: Armazenamento de senhas, strings de conexão e outros dados confidenciais.
- Chaves criptográficas: Gerenciamento de chaves para assinatura e criptografia.
- Certificados: Gerenciamento de certificados SSL/TLS.
**Benefícios:**
- Integração com serviços do Azure para autenticação automatizada via Identidades Gerenciadas.
- Rotação automática de segredos e chaves.

## Armazenamento 
O Azure Blob Storage é usado para armazenar grandes volumes de dados não estruturados.

**Tipos de Blobs:**
- Blobs de blocos: Para armazenamento de arquivos, como imagens e vídeos.
- Blobs de páginas: Otimizados para dados acessados frequentemente (discos virtuais).
- Blobs de anexos: Para armazenamento de logs ou backups.
**Exemplos de uso:**
- Hospedagem de arquivos estáticos para aplicativos web.
- Armazenamento de backups de banco de dados.

## Configuração Centralizada 
O Azure App Configuration oferece:

- Centralização de configurações para vários ambientes.
- Integração com Azure Key Vault para gestão de segredos.
- Gerenciamento de feature flags para controle de funcionalidades em produção.
**Caso de uso:**
Alterar configurações de um aplicativo sem a necessidade de reinicialização ou implantação.

## Mensageria e Filas 
**Azure Service Bus**
- Serviço de mensageria para comunicação assíncrona entre serviços.
- Suporte para filas e tópicos (pub/sub).
**Azure Event Grid**
- Gerenciamento de eventos em larga escala.
- Integração com serviços como Azure Functions e Logic Apps.
**Exemplos de uso:**
- Service Bus: Processar ordens de compra em uma fila para escalabilidade.
- Event Grid: Disparar eventos para funções serverless ao carregar um arquivo no Blob Storage.

## Monitoramento e Diagnóstico 
**Azure Monitor**
- Coleta e análise de logs e métricas de desempenho.
**Application Insights**
- Monitoramento de desempenho de aplicativos em tempo real.
- Identificação de gargalos e problemas de latência.

**Caso de uso:**
Monitorar um aplicativo web para identificar consultas de banco de dados lentas e erros de API.

## Desenvolvimento e Implementação 
**Azure Functions**
- Serviço serverless para execução de código em resposta a eventos.
- Suporte para linguagens como C#, Python, JavaScript, entre outras.
**Azure App Services**
- Hospedagem de aplicativos web e APIs com alta disponibilidade.
- Suporte para implantações contínuas usando GitHub Actions ou Azure DevOps.
**Exemplos de uso:**
- Azure Functions: Executar um script de limpeza após um arquivo ser enviado ao Blob Storage.
- Azure App Services: Hospedar uma API REST para um aplicativo mobile.

## Recursos Adicionais
- Certificação AZ-204: [Documentação oficial](https://learn.microsoft.com/en-us/credentials/certifications/azure-developer/?practice-assessment-type=certification)
- Exemplos de implementação no GitHub:
  - [Gerenciamento de APIs](https://github.com/Azure/api-management-samples)
  - [Azure Functions](https://github.com/Azure/azure-functions-host)

Este README cobre serviços essenciais para desenvolvedores no Azure, ajudando a construir soluções seguras, escaláveis e eficientes. Explore os links adicionais para aprofundar seu conhecimento!
