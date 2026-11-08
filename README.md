# Guia de Publicação e Verificação de Empresa na Meta

Este repositório contém a estrutura completa do site institucional e das páginas jurídicas necessárias para aprovar a **Verificação da Empresa (Business Verification)** e configurar o **Aplicativo de Desenvolvedor da Meta (Tech Provider / WhatsApp Embedded Signup)**.

Todos os dados fiscais e cadastrais inseridos estão **100% alinhados com o seu CCMEI oficial**:
* **Razão Social:** `70.031.884 PEDRO HENRIQUE BARBOSA GUTIERRES`
* **CNPJ:** `70.031.884/0001-27`
* **Endereço:** `Rua Engenheiro Gama Lobo, 548, Bloco 5, Apt 102 - Vila Isabel, Rio de Janeiro - RJ, CEP 20551-100`

---

## 📁 Arquivos Criados

* `index.html`: Landing page moderna e responsiva (Tailwind CSS) apresentando a solução de automação no WhatsApp com IA e rodapé com os dados cadastrais completos.
* `politica-de-privacidade.html`: Política de Privacidade em total conformidade com a LGPD, Meta Developer Policies e instruções de exclusão de dados.
* `termos-de-uso.html`: Termos de Serviço com diretrizes anti-SPAM e conformidade com as regras do WhatsApp Business.

---

## 🚀 Como Publicar Gratuitamente no Cloudflare Pages

Como você já planeja usar a Cloudflare para o Worker, o **Cloudflare Pages** é a melhor opção:

### Método 1: Upload Direto (Mais Rápido - 1 minuto)
1. Acesse o painel da [Cloudflare](https://dash.cloudflare.com/).
2. Vá em **Compute (Workers & Pages)** > **Create application** > aba **Pages**.
3. Selecione a opção **Upload assets**.
4. Defina o nome do projeto (ex.: `gutierrestech` ou o nome que preferir).
5. Arraste a pasta deste projeto (`d:\automacaoatendimento`) para a área de upload.
6. Clique em **Deploy site**.
7. Seu site estará no ar instantaneamente em `https://seu-projeto.pages.dev`.

### Método 2: Conectar seu Domínio Próprio
1. No painel do seu projeto no Cloudflare Pages, vá na aba **Custom domains**.
2. Clique em **Set up a custom domain** e digite o seu domínio (ex.: `seudominio.com.br`).
3. O Cloudflare gerencia o SSL (HTTPS) de forma automática e gratuita.

---

## 🛡️ Passo a Passo para Aprovação na Meta

### 1. Verificação do Domínio na Meta
1. Acesse o [Gerenciador de Negócios da Meta](https://business.facebook.com/settings/).
2. Vá em **Adequação e Segurança da Marca** > **Domínios**.
3. Clique em **Adicionar** > **Criar um novo domínio** e informe seu domínio (sem `https://`).
4. Escolha o método **Registro TXT do DNS**:
   * Copie o código `facebook-domain-verification=...`.
   * Abra o painel da Cloudflare na aba **DNS** do seu domínio.
   * Crie um registro tipo `TXT`, nome `@`, valor com o código da Meta e salve.
5. Volte na Meta e clique em **Verificar Domínio**.

### 2. Iniciar a Verificação da Empresa
1. No Gerenciador de Negócios, vá em **Centro de Segurança** > **Verificação da Empresa** e clique em **Iniciar Verificação**.
2. Preencha os campos com os dados exatos do seu CCMEI:
   * **Nome legal da empresa:** `70.031.884 PEDRO HENRIQUE BARBOSA GUTIERRES`
   * **Endereço:** `Rua Engenheiro Gama Lobo, 548, Bloco 5, Apt 102`
   * **Cidade:** `Rio de Janeiro`
   * **Estado:** `RJ`
   * **CEP:** `20551-100`
   * **Site:** `https://seudominio.com.br`
3. Anexe o documento oficial em PDF do **CCMEI** (Certificado de MEI).
4. Selecione a confirmação por **E-mail corporativo** (`contato@seudominio.com.br`) ou SMS/ligação.

### 3. Configurar no Meta for Developers (App do WhatsApp)
1. Acesse o [Meta for Developers](https://developers.facebook.com/apps/).
2. Abra seu aplicativo do tipo **Negócios (Business)**.
3. Em **Configurações Básicas**:
   * **URL da Política de Privacidade:** `https://seudominio.com.br/politica-de-privacidade.html`
   * **URL dos Termos de Serviço:** `https://seudominio.com.br/termos-de-uso.html`
   * **Domínio do Aplicativo:** `seudominio.com.br`
   * **Ícone do Aplicativo:** Faça upload de uma logo com 1024x1024 px.
