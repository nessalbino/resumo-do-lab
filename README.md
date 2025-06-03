# Anotações aulas 
## Aula sobre Introdução a computação em Nuvem

## Nuvem Pública
- Nenhuma despesa de capital para escalar verticalmente.
- As organizações pagam apenas pelo que utilizam.


## Nuvem Privada
- As organizações têm controle total sobre os recursos e a segurança.
- As organizações são responsáveis pela manutenção e pelas atualizações de hardware e software.

## Nuvem Híbrida
  - As organizações determinam onde executar seus aplicativos.
  - As organizações controlam a segurança, a conformidade e os requisitos legais.
  - Fornece maior flexibilidade.
 
## CapEx
Despesa de Capital (CapEx)
- O gasto inicial de dinheiro em insfraestrutura física.
- As despesas do CapEx têm um valor que se reduz com o tempo.
   
## OpEx
Despesas operacionais (OpEx)
- Gastar com produtos e serviçoos conforme necessário, pagamento conforme o uso.
- Seja cobrado imediatamente.

--------------------------------------------------------------

## Benefícios da Computação em Nuvem

- Alta disponibilidade > Garantir a disponibilidade máxima
- Escalabilidade > Capacidade de adicionar mais recursos para lidar melhor com o aumento da demanda. Paga apenas pelo que usa.
- Elasticidade > seus recursos implantados poderiam ser expandidos (automaticamente ou manualmente) caso você tenha um salto repentino acentuado na demanda. E reduzidos caso aja uma queda na demanda.
      Ex. você pode adicionar maquinas virtuais ou contêiners por meio da expansão.
- Confiabilidade > Com um design descentralizado, a nuvem permite que você tenha recursos implantados em várias regiões do mundo.
- Previsibilidade > Permite que você avance com confiança, seja no desempenho ou no custo. Ambas influenciadas pelo Microsoft Azure Well-Architected Framework.
- Segurança - A nuvem oferece ferramentas de segurança que atendem às necessidades dos clientes (devem ser realizadas pelo cliente).
- Governança - Dependendo do modelo operacional, patches de software e atualizações podem ser aplicados automaticamente, o que ajuda na governança e na segurança.
- Gerenciabilidade - Gerenciamento do ambiente e dos recursos em nuvem.
      Ex. Escalar automaticamente a implantação de recursos com base na necessidade.
          Por meio de um portal Web.
          Usando interface de linha de comando, APIs, PowerShell

  ----------------------------------------------------------

  # Tabela SLA

  ![image](https://github.com/user-attachments/assets/eafaf65b-00a7-4aff-bf3f-684cb35448fe)

  ---------------------

  # Tipos de Serviços
    ## IaaS - Infraestrutura como Serviço
  Fornece: Recursos de infraestrutura como servidores, armazenamento, redes e sistemas operacionais.

  Usuário gerencia:Sistema operacional, aplicações, dados

  Escalabilidade: Alta, com pagamento sob demanda

    ## PaaS - Plataforma como Serviço

  Fornece: Plataforma com sistema operacional, banco de dados, middleware e ferramentas de desenvolvimento.

  Usuário Gerencia: Apenas os aplicativos e dados

  Produditividade: Alta, com foco no desenvolvimento sem se preocupar com a infraestrutura.

    ## SaaS - Software como Serviçco

  Fornece: Aplicativos completos prontos para uso, acessados via internet.

  Usuário gerencia: Apenas o uso da aplicação

  Facilidade de uso: Alta, sem necessidade de instalação ou manutenção.

  
  ## Modelo de Responsabilidade Compartilhada

  ![image](https://github.com/user-attachments/assets/c7efa3ba-5c40-4ba7-8df1-f02d4ec9f4ef)

  ## Zona de Disponibilidade


![image](https://github.com/user-attachments/assets/49fdf520-a09e-468d-bc9f-3ece37fffc2d)

  ## Serviço de Computação do Azure

  A computação Azure é um serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais.

  ## Máquinas Virtuais do Azure

  As máquinas virtuais do Azure (VMs) são emulações de Software de computadores físicos.
  Inclui: Processador Virtual, Memória, Armazenamento e Rede.
  Oferta de Iaas que oferece personalização e controle total

  ## Conjunto de Dimensionamento de VMs
  Os conjuntos de dimensionamento oferece uma oportunidade de balanceamento de carga para dimensionar os recursos automaticamente.
    * Escalar horizontalmente quando o recurso precisar aumentar, reduzir quando precisa diminuir.

  ## Área de Trabalho Virtual do Azure
  É uma virtualização da área de trabalho e aplicativo executada na nuvem.
  Crie um ambiente completo de virtualização da área de trabalho sem precisar executar outros servidores de gateway.
  Reduza o risco de que o recurso seja deixado para trás.
  Implantações reais de várias sessões.

  ## Serviços de Contêineres do Azure
  Serviços de Contêineres do Azure são opções que o Azure oferece para executar e gerenciar contêineres (como os do Docker) na nuvem.

  Em outras palavras:
  Eles permitem que você rode suas aplicações empacotadas em contêineres de forma fácil, escalável e segura.
  
  Principais opções:
  Azure Container Instances (ACI):
  Roda contêineres rapidamente, sem precisar gerenciar servidores. Ideal para cargas leves ou temporárias.
  
  Azure Kubernetes Service (AKS):
  Uma plataforma mais robusta que usa Kubernetes para orquestrar e gerenciar muitos contêineres ao mesmo tempo. Ideal para aplicações grandes e complexas.
  
  Vantagens:
  Roda aplicações de forma isolada e portátil.
  Escalabilidade automática.
  Menos preocupação com infraestrutura.
  
  ## Aplicativos de Contêineres do Azure
  Uma oferta de PaaS, como instâncias de contêineres que pode balancear a carga e escalar.
  Servições de Kubernetes do Azure: Um serviço de orquestração para contêineres com arquitetura distribuídas e grande volumes de contêineres.

  ## Azure Functions
  Azure Functions é um serviço da Microsoft Azure que permite rodar pequenos pedaços de código (chamados de "funções") na nuvem sem precisar se preocupar com servidores.
  Em outras palavras:
  Você escreve uma função (ex: em C#, JavaScript, Python, etc).
  Sobe essa função para o Azure.
  O Azure executa essa função automaticamente quando algo acontece (como um envio de arquivo, uma requisição HTTP, uma mensagem em fila, etc).
  Você paga apenas pelo tempo de execução, ou seja, quando a função é usada.

  ## Serviços de Rede do Azure
  Serviços de Rede do Azure são ferramentas e recursos que ajudam a conectar, proteger e distribuir suas aplicações na nuvem e fora dela.

  Em outras palavras:
  Eles permitem que seus sistemas se comuniquem com segurança e eficiência, tanto entre si quanto com usuários.
  
  Principais serviços:
  Azure Virtual Network (VNet):
  Cria uma rede privada na nuvem, como se fosse uma rede local, para conectar recursos do Azure.
  
  Azure Load Balancer:
  Distribui o tráfego entre vários servidores para garantir alta disponibilidade.
  
  Azure Application Gateway:
  Gerencia tráfego de aplicações web e oferece firewall de aplicativo (WAF).
  
  Azure VPN Gateway:
  Conecta redes locais (físicas) ao Azure por meio de uma VPN segura.
  
  Azure ExpressRoute:
  Conexão dedicada e mais rápida entre sua infraestrutura local e o Azure (sem passar pela internet pública).
  
  Azure DNS:
  Gerencia nomes de domínio com alta disponibilidade e desempenho.
  
  Vantagens:
  Comunicação segura entre recursos.
  Melhor desempenho e escalabilidade.
  Alta disponibilidade e proteção contra falhas.

## DSN do Azure
  Azure DNS é um serviço do Azure que permite gerenciar nomes de domínio (como meusite.com) usando a infraestrutura da Microsoft.
  Em outras palavras:
  Ele converte nomes de sites em endereços IP (o que os computadores entendem), de forma rápida e confiável.
  
  O que dá pra fazer com ele:
  Criar e gerenciar registros DNS (como A, CNAME, MX, etc).
  Apontar seu domínio para sites, APIs ou outros serviços.
  Usar a infraestrutura global do Azure, garantindo alta performance.
  
  Vantagens:
  Rápido e confiável.
  Fácil integração com outros serviços do Azure.
  Alta disponibilidade (quase sempre online).
  
  Obs: O Azure DNS não registra domínios, apenas gerencia os registros de domínios que você já possui.
  
    

  
  
  
  

  

  
  

  
  

          
          
          
          
  


 
