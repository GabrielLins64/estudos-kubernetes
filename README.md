<h2>Kubernetes</h2>

Material de estudo desenvolvido através da formação de Kubernetes da alura e da leitura da documentação oficial do Kubernetes.

---

- [Termos importantes](#termos-importantes)
- [O que é Kubernetes](#o-que-é-kubernetes)
- [Objetos do Kubernetes](#objetos-do-kubernetes)
- [Clusters](#clusters)
- [Referências](#referências)

---

## Termos importantes

- **Escalabilidade horizontal:**

  > Adicionar mais unidades de recurso (como servidores ou contêineres) para distribuir a carga de trabalho.

- **Escalabilidade vertical:**

  > Aumentar a capacidade de uma única unidade de recurso (como adicionar mais CPU ou memória a um servidor).

- **Cluster:**
  > é um conjunto de máquinas (nós) que trabalham juntas para executar aplicações em contêineres.

---

## O que é Kubernetes

Kubernetes é uma plataforma portátil, extensível e de código aberto para gerenciar cargas de trabalho e serviços em contêineres, que facilita tanto a configuração declarativa quanto a automação. Ele possui um ecossistema grande e em rápido crescimento. Serviços, suporte e ferramentas para Kubernetes estão amplamente disponíveis.

O nome Kubernetes origina-se do grego, significando timoneiro ou piloto. K8s como uma abreviação resulta da contagem das oito letras entre o "K" e o "s". O Google disponibilizou o projeto Kubernetes como código aberto em 2014. Kubernetes combina mais de 15 anos de experiência do Google na execução de cargas de trabalho de produção em grande escala com as melhores ideias e práticas da comunidade.

Kubernetes oferece:

- **Descoberta de serviços e balanceamento de carga**
  Kubernetes pode expor um contêiner usando o nome DNS ou seu próprio endereço IP. Se o tráfego para um contêiner for alto, o Kubernetes é capaz de balancear a carga e distribuir o tráfego de rede para que a implantação seja estável.

- **Orquestração de armazenamento**
  Kubernetes permite que você monte automaticamente um sistema de armazenamento de sua escolha, como armazenamentos locais, provedores de nuvem pública e outros.

- **Implantações e reversões automatizadas**
  Você pode descrever o estado desejado para seus contêineres implantados usando Kubernetes, e ele pode mudar o estado atual para o estado desejado em uma taxa controlada. Por exemplo, você pode automatizar o Kubernetes para criar novos contêineres para sua implantação, remover contêineres existentes e adotar todos os recursos para o novo contêiner.

- **Ajuste automático de bin**
  Você fornece ao Kubernetes um cluster de nós que ele pode usar para executar tarefas em contêineres. Você informa ao Kubernetes quanto de CPU e memória (RAM) cada contêiner precisa. O Kubernetes pode ajustar os contêineres nos seus nós para fazer o melhor uso dos seus recursos.

- **Auto-recuperação**
  Kubernetes reinicia contêineres que falham, substitui contêineres, mata contêineres que não respondem às verificações de saúde definidas pelo usuário e não os anuncia para os clientes até que estejam prontos para servir.

- **Gerenciamento de segredos e configurações**
  Kubernetes permite que você armazene e gerencie informações sensíveis, como senhas, tokens OAuth e chaves SSH. Você pode implantar e atualizar segredos e a configuração da aplicação sem reconstruir suas imagens de contêiner e sem expor segredos na configuração da pilha.

- **Execução em lote**
  Além de serviços, Kubernetes pode gerenciar suas cargas de trabalho de lote e CI, substituindo contêineres que falham, se desejado.

- **Escalonamento horizontal**
  Escalone sua aplicação para cima e para baixo com um comando simples, com uma interface de usuário, ou automaticamente com base no uso de CPU.

- **Pilha dupla IPv4/IPv6**
  Alocação de endereços IPv4 e IPv6 para Pods e Serviços.

- **Projetado para extensibilidade**
  Adicione recursos ao seu cluster Kubernetes sem alterar o código-fonte upstream.

---

## Objetos do Kubernetes

---

## Clusters

No contexto de Kubernetes, um cluster é um conjunto de máquinas (nós) que trabalham juntas para executar aplicações em contêineres. O cluster é composto por:

- **Nó mestre (ou nós mestres)**: Gerencia o cluster, coordenando todas as atividades, como a programação dos contêineres, a manutenção do estado desejado das aplicações e a implementação das atualizações.

- **Nós de trabalho**: Executam as aplicações em contêineres. Cada nó de trabalho pode conter um ou mais contêineres gerenciados pelo Kubernetes.

Os componentes principais de um cluster Kubernetes incluem o servidor de API, o controlador, o gerenciador de estados, o kubelet, o kube-proxy e o etcd (banco de dados chave-valor). Juntos, eles garantem que as aplicações sejam executadas de forma eficiente, escalável e resiliente.

---

## Referências

[1] [Documentação Oficial do Kubernetes](https://kubernetes.io/docs/home/)

[2] [Formação Kubernetes Alura](https://cursos.alura.com.br/formacao-kubernetes)
