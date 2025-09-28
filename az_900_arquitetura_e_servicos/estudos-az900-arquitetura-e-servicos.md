
# Arquitetura e Serviços Azure

1. [Introdução ao a Microsoft Azure](#introdução-a-microsoft-azure)

2. [Construindo Arquiteturas no Azure](#construindo-arquiteturas-no-azure)

3. [Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure](#configurando-recursos-e-dimensionamentos-em-máquinas-virtuais-na-azure)

4. [Dominando o Armazenamento na Azure](#dominando-o-armazenamento-na-azure)

5. [Entendendo sobre Segurança e Identidade na Azure](#entendendo-sobre-segurança-e-identidade-na-azure)

---

1. ### Introdução a Microsoft Azure

Guia disponibilizado pela própria Microsoft para iniciantes e entusiastas de computação em nuvem. [Introdução Azure](https://learn.microsoft.com/pt-br/training/paths/microsoft-azure-fundamentals-describe-cloud-concepts/)

2. ### Construindo Arquiteturas no Azure

A arquitetura da Azure segue o modelo em camadas:
Na camada mais baixa encontram-se os datacenters que estão contidos em uma Região.
No ecossistema da Azure uma região é um espaço geográfico onde existe um ou mais datacenters que estão conectados por meio de redes de baixa latência.
Uma região contém Zonas de disponibilidade que são datacenters dentro da mesma região porém separados fisicamente, auxiliando no processo de recuperação de desastres.
A Azure utiliza a abordagem de pares de regiões onde duas regiões distantes a pelo menos 300 milhas (480km), para comutação em caso de desastres.
Este descritivo mostra como a Azure se estrutura de forma física.

Na parte lógica da Azure a arquitetura inclui recursos do Azure e grupos de recursos, assinaturas e contas.

**Recurso**: Um recurso é o bloco de construção básico do Azure. Qualquer coisa que você criar, provisionar, implantar etc. é um recurso. VMs (máquinas virtuais), redes virtuais, bancos de dados, serviços cognitivos etc. são todos considerados recursos no Azure

**Grupos de recursos**: Os grupos de recursos são simplesmente agrupamentos de recursos. Quando você cria um recurso, é necessário colocá-lo em um grupo de recursos. **Observação**: Embora um grupo de recursos possa conter muitos recursos, apenas um recurso pode estar em um grupo de recursos por vez.

**Assinaturas**: as assinaturas são uma unidade de gerenciamento, cobrança e escala. Semelhante a como os grupos de recursos são um modo de organizar logicamente os recursos, as assinaturas permitem organizar logicamente seus grupos de recursos e facilitar a cobrança.

**Contas**: são contas para utilização da infraestrutura da Azure.

###### fonte: [(Microsoft, 2025)](https://learn.microsoft.com/pt-br/training/modules/describe-core-architectural-components-of-azure/)


3. ### Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure

Na Azure é possível criar recursos com configurações pré-definidas ou soluções completas com base nas opções do portal da Azure.
Para criar recursos com base nos requisitos específicos da organização [acesse.](https://learn.microsoft.com/pt-br/azure/virtual-machines/overview)
Mais informações sobre o significado de cada  atributo para ser preenchido em: [Virtual Machine](https://learn.microsoft.com/pt-br/training/modules/create-windows-virtual-machine-in-azure/2-create-a-windows-virtual-machine)
**Azure Functions** [Em breve].

4. ### Dominando o Armazenamento na Azure

Uma conta de armazenamento fornece um namespace exclusivo (nome deve ser único e devem ter entre 3 e 24 caracteres e podem conter apenas números e letras minúsculas.) para os dados do Armazenamento do Azure que podem ser acessados de qualquer lugar do mundo por HTTP ou HTTPS

Ao criar uma conta de armazenamento, você começará escolhendo o tipo da conta de armazenamento. O tipo de conta determina os serviços de armazenamento e as opções de redundância e tem impacto nos casos de uso.
-   LRS (armazenamento com redundância local)
-   Armazenamento com redundância geográfica (GRS)
-   RA-GRS (armazenamento com redundância geográfica com acesso de leitura)
-   ZRS (armazenamento com redundância de zona)
-   Armazenamento com redundância de zona geográfica (GZRS)
-   RA-GZRS (armazenamento com redundância de zona geográfica com acesso de leitura)
- 
**Observação**: Estudar significado dos atributos preenchidos.
###### fonte:[(Microsoft, 2025)](https://learn.microsoft.com/pt-br/training/modules/describe-azure-storage-services/ )

5. ### Entendendo sobre Segurança e Identidade na Azure

O Microsoft Entra ID é um serviço de diretório que permite que você faça login e acesse tanto os aplicativos de nuvem da Microsoft quanto os aplicativos de nuvem que você desenvolver. O Microsoft Entra ID também pode ajudar você a manter sua implantação do Active Directory local

O Microsoft Entra ID fornece serviços como:

-   **Autenticação**: inclui verificar a identidade para acessar aplicativos e recursos. Também inclui fornecer funcionalidades como redefinição de senha por autoatendimento, autenticação multifator, uma lista personalizada de senhas banidas e serviços de bloqueio inteligente.
-   **Logon único**: o SSO (logon único) permite que você se lembre apenas de um nome de usuário e uma senha para acessar vários aplicativos. Uma única identidade é vinculada a um usuário, o que simplifica o modelo de segurança. À medida que os usuários trocam de funções ou saem de uma organização, as modificações de acesso são vinculadas àquela identidade, o que reduz consideravelmente o esforço necessário para alterar ou desabilitar contas.
-   **Gerenciamento de aplicativos**: Você pode gerenciar seus aplicativos de nuvem e locais usando o Microsoft Entra ID. Recursos como Proxy de Aplicativo, aplicativos SaaS, o portal Meus Aplicativos e o logon único proporcionam uma experiência do usuário aprimorada.
-   **Gerenciamento de dispositivos**: Além de seu uso com as contas individuais de uma pessoa, o Microsoft Entra ID dá suporte ao registro de dispositivos. O registro permite que os dispositivos sejam gerenciados por meio de ferramentas como o Microsoft Intune. Também permite que políticas de Acesso Condicional baseadas no dispositivo restrinjam tentativas de acesso somente às provenientes de dispositivos conhecidos, independentemente da conta de usuário solicitante.
###### fonte:[(Microsoft, 2025)](https://learn.microsoft.com/pt-br/training/modules/describe-azure-identity-access-security/)
