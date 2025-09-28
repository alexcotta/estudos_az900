
# Conceitos Iniciais de Cloud com Azure

## Introdução ao Ambiente Cloud
1. [Introdução ao a Microsoft Azure](#introdução-a-microsoft-azure)

2. [Microsoft Azure Localizando Serviços por Categoria](#microsoft-azure-localizando-serviços-por-categoria)

3. [Criando máquinas Virtuais na Azure](#criando-máquinas-virtuais-na-azure)

4. [Configurando uma instância de Banco de Dados na Azure](#configurando-uma-instância-de-banco-de-dados-na-azure)

---

1.  ### Introdução a Microsoft Azure

Guia disponibilizado pela própria Microsoft para iniciantes e entusiastas de computação em nuvem. [Introdução Azure](https://learn.microsoft.com/pt-br/training/paths/microsoft-azure-fundamentals-describe-cloud-concepts/)

2. ### Microsoft Azure Localizando Serviços por Categoria


![Painel principal do Microsoft Azure](https://learn.microsoft.com/pt-br/azure/azure-portal/media/azure-portal-overview/portal-callouts.png "Menu principal do Azure")
###### fonte: [(Microsoft, 2025)](https://learn.microsoft.com/pt-br/azure/azure-portal/azure-portal-overview)

| Chave   | Descrição     |   
|---|---|
|  1 | Menu do portal. Esse elemento global pode ajudá-lo a navegar entre serviços. Aqui, o menu do portal está no modo de submenu, portanto, ele ficará oculto até que você selecione o ícone de menu.  |
| 2  |  **Trilha**. Use os links de trilha para voltar um nível no fluxo de trabalho. |
| 3  | **Cabeçalho da página**. Aparece na parte superior de todas as páginas do portal e contém elementos globais.  | 
| 4  | **Pesquisa global**. Use a barra de pesquisa no cabeçalho de página para localizar rapidamente um recurso, um serviço ou uma documentação específica.
| 5  | **Copilot**. Fornece acesso rápido ao [Microsoft Copilot no Azure (versão prévia)](https://learn.microsoft.com/pt-br/azure/copilot/).
| 6  | **Controles globais**. Esses controles para tarefas comuns persistem no cabeçalho da página: Cloud Shell, Notificações, Configurações, Suporte + Solução de Problemas e Comentários.
| 7  | **Sua conta**. Veja informações sobre sua conta, alterne entre diretórios, saia ou entre com uma conta diferente.
| 8  | **Barra de comandos**. Um grupo de controles que são contextuais para seu foco atual.
| 9  | **[Menu de serviço](https://learn.microsoft.com/pt-br/azure/azure-portal/azure-portal-overview#service-menu)**. Um menu com comandos contextuais para o serviço ou recurso com o qual você esteja trabalhando. Às vezes, é chamado de menu de recursos.
| 10 | **Painel de trabalho**. Exibe detalhes sobre o recurso ou o serviço que está em foco no momento.

No menu do portal [1] é possível acessar as principais funcionalidades e tipos de recursos inclusive os serviços disponibilizados pela Azure.




3. ### Criando máquinas Virtuais na Azure

Os passos para criar uma máquina virtual na Azure utilizando o exemplo do Windows Server são:

1.  Entre no [portal do Azure](https://portal.azure.com/learn.docs.microsoft.com) usando a mesma conta usada para ativar a área restrita.
    
2.  No portal do Azure, em **Serviços do Azure**, selecione **Criar um recurso**. O painel **Criar um recurso** será exibido.
    
3.  Na caixa de pesquisa _Pesquisar serviços e marketplace_, procure _Windows Server_ e pressione Enter. Selecione **Windows Server** fornecido pela Microsoft. O painel **Windows Server** é exibido.
    
4.  Há várias opções de Windows Server para criar a VM. Na lista suspensa **Plano**, role para baixo e selecione **[smalldisk] Windows Server 2019 Datacenter**.
    
5.  Selecione **Criar**. O painel **Criar uma máquina virtual** aparece.

Dentre as configurações da máquina virtual ressalta-se a necessidade de se escolher a região onde a máquina será criada e a disponibilidade necessária para máquina. 

Estas configurações impactam diretamente no uso da VM uma vez que caso uma região sua VM fique indisponível será redirecionado o acesso para uma outra região. Escolher as melhores opções de disponibilidade impactam diretamente no valor a ser pago e devem ser planejadas previamente.

###### fonte:[(Microsoft, 2025)](https://learn.microsoft.com/pt-br/training/modules/create-windows-virtual-machine-in-azure/)






4. ### Configurando uma instância de Banco de Dados na Azure

Para criar uma instancia de banco de dados na Azure é possivel através do portal, powershell e cli do azure como exemplo será utilizado os passos dentro do portal da Azure

1.   Entre no [portal do Azure](https://portal.azure.com/).
    
2. Vá para o [Hub SQL do Azure em aka.ms/azuresqlhub](https://aka.ms/azuresqlhub).
    
3. No painel da **Instância Gerenciada de SQL do Azure**, selecione **Mostrar opções**.
    
4. Na janela de **opções da Instância Gerenciada de SQL do Azure** , selecione **Criar Instância Gerenciada de SQL**.

Configurações adicionais podem ser conferidas no link da fonte

###### fonte: [(Microsoft, 2025)](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/instance-create-quickstart?view=azuresql&tabs=azure-portal)


