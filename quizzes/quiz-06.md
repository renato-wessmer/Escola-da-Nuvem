## Quiz 06

#### Q1. A URL de um álbum de fotos compactado foi compartilhada por e-mail para um cliente, mas ele informou que ao acessar apresenta o erro Access Denied. Como corrigir? (Selecione 2)

- [ ] Tornar bucket privado
- [x] Tornar Bucket público
- [x] Adicionar uma Política ao Bucket
- [ ] Habilitar versionamento

#### Q2. Qual serviço utilizamos para criar um repositório de data lake?  

- [x] S3
- [ ] EC2
- [ ] EBS
- [ ] Snowmobile

#### Para criar um repositório de data lake, um serviço comumente utilizado é o Amazon S3 (Simple Storage Service), que é um serviço de armazenamento em nuvem escalável (aumentar ou diminuir o tamanho do seu repositório de data lake), durável, para armazenar grandes quantidades de dados (estruturados, semiprocessados e processados) com capacidade de armazenar e recuperar qualquer quantidade de dados.                                                   O EC2 (Elastic Compute Cloud) é um serviço de computação em nuvem que permite executar aplicativos em máquinas virtuais escaláveis, já o EBS (Elastic Block Store) é um serviço de armazenamento de blocos persistentes para uso com instâncias do EC2 e o Snowmobile é um serviço de transferência de grandes volumes de dados de uma infraestrutura local para a nuvem com capacidade de até 100 PB (petabytes) de dados.

#### Q3. Qual destes armazenamentos permite a instalação de um sistema operacional?

- [x] EBS
- [ ] S3
- [ ] Glacier Deep Archive
- [ ] S3 Website estático

#### O único armazenamento que permite a instalação de um sistema operacional é o EBS (Elastic Block Store), com o EBS pode-se criar um volume de armazenamento e anexá-lo a uma instância do EC2 como um disco rígido virtual, sendo que o volume pode ser formatado com um sistema de arquivos e pode conter um sistema operacional completo (Linux ou o Windows), assim podendo-se inicializar uma instância do EC2 diretamente do volume do EBS executando um sistema operacional completo.                                                                                                           O S3 (Simple Storage Service) é um serviço projetado para armazenar e recuperar dados, já o Glacier Deep Archive é um serviço de armazenamento de longo prazo, para dados que não precisam de acesso imediato, ou seja, é otimizado para o armazenamento de dados que raramente são acessados, e, S3 Website estático é uma funcionalidade do S3 que permite a hospedagem de sites estáticos, como páginas HTML, CSS e JavaScript. 

#### Q4. Qual destes armazenamentos NÃO permite a recuperação de um objeto imediatamente?

- [ ] S3 IA (Infrequent Access)
- [ ] S3 Standard
- [ ] S3 Intelligent Tiering
- [x] S3 Glacier Deep Archive

#### O armazenamento que não permite a recuperação imediata é o S3 Glacier Deep Archive, projetado para o armazenamento em nuvem de longo prazo, ou seja, que raramente são acessados, a recuperação pode levar algumas horas até estar disponível para recuperação, sendo esse intervalo conhecido como recuperação em várias etapas.             O S3 IA (Infrequent Access) e o S3 Standard já são classes de armazenamento que permitem a recuperação imediata de objetos, já o S3 Intelligent Tiering é uma classe de armazenamento que utiliza aprendizado de máquina para analisar os padrões de acesso aos dados e automaticamente mudar os objetos entre as classes de armazenamento com objetivo de otimizar custos e manter a recuperação imediata dos objetos.

#### Q5. Algum funcionário está apagando os objetos dos buckets sem querer e você precisa recuperar esses objetos rapidamente. Qual característica do Amazon S3 podemos utilizar em casos assim?

- [ ] Tornar bucket privado
- [ ] Tornar Bucket público
- [ ] Tornar objeto como público
- [x] Habilitar versionamento

#### O versionamento (versioning) no bucket, faz com que cada objeto armazenado no bucket recebe uma versão única, ou seja, ao invés de substituir o objeto existente quando uma nova versão é enviada, se mantém todas as versões anteriores do objeto, assim mesmo que um objeto seja excluído, ele não será permanentemente removido podendo se escolher a versão específica que deseja recuperar.                                                                  O bucket privado, o bucket público ou tornar um objeto como público são configurações de acesso ao bucket ou objeto.

#### Q6. Uma papelaria precisa criar um website estático para compartilharem fotos da loja e telefones de contato. Qual destes serviços atende a esta solicitação?

- [ ] EBS
- [ ] Glacier
- [x] S3
- [ ] Glacier Deep Archive

#### O Amazon S3 é projetado para armazenar e fornecer acesso a uma ampla variedade de dados, incluindo arquivos estáticos, como páginas HTML, imagens, vídeos e documentos, dessa forma, pode-se criar um website estático sem a necessidade de gerenciar uma infraestrutura de servidor complexa, permitindo também o controle de acesso para os arquivos armazenados.

#### Q7. Qual o nome da característica do S3 que realiza a movimentação de objetos entre armazenamentos?

- [ ] S3 Deep Archive
- [x] Ciclo de Vida
- [ ] Snowball
- [ ] AWS Database Migration Service
  
#### A característica do Amazon S3 que realiza a movimentação de objetos entre armazenamentos é chamada de "Ciclo de Vida" (Lifecycle).

O Ciclo de Vida do S3 é uma funcionalidade que permite automatizar a movimentação de objetos entre as classes de armazenamento do S3, como S3 Standard, S3 Intelligent-Tiering e S3 Glacier, com base em regras predefinidas.

Com o Ciclo de Vida, é possível definir regras para determinar quando e como os objetos são movidos entre as classes de armazenamento. Por exemplo, você pode configurar uma regra para mover objetos para uma classe de armazenamento de custo mais baixo, como o S3 Intelligent-Tiering ou o S3 Glacier, após um determinado período de tempo em que os objetos não são acessados com frequência.

Essa funcionalidade ajuda a otimizar os custos de armazenamento, permitindo que você utilize as classes de armazenamento adequadas para cada estágio do ciclo de vida dos seus dados, movendo automaticamente os objetos para armazenamentos mais econômicos à medida que sua frequência de acesso diminui.

Portanto, o recurso do Amazon S3 que realiza a movimentação de objetos entre armazenamentos é o Ciclo de Vida.


#### Q8. Um funcionário não está conseguindo criar um bucket S3. Qual o motivo?

- [x] Não possui nome único global
- [ ] O bucket está privado
- [ ] O bucket está público
- [ ] Precisa habilitar o versionamento

#### Q9. Você foi chamado para uma reunião porque o banco de dados no Amazon EC2 não está como um bom desempenho. Após olhar a instância você identificou ser preciso trocar o tipo de armazenamento por um com maior performance. Qual das opções abaixo oferece o maior performance?

- [ ] GP3
- [ ] Magnético
- [x] IO2
- [ ] GP2

#### Q10. Você precisa executar poder computacional na borda e depois migrar 39 TB para a Nuvem. Qual o melhor armazenamento de migração escolher?

- [ ] Snowball Edge Storage Optimized
- [x] Snowball Edge Compute Optimized
- [ ] Snowcone
- [ ] Snowmobile
