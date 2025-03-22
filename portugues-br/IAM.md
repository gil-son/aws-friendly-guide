IAM

<div align="center">
  <img src="https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/aws-cloud-security/control-access-with-aws-identity-and-access-management/images/3d5ecfeab35e8dfc1eb781f7880fafc9_99-c-15-ccc-fe-5-e-4-d-8-f-bcfc-193197-b-9-dc-7-b.png" width="25%">
</div>
<br/>

O AWS <b>Identity and Access Management - IAM </b> é um dos principais recursos, pois permite o gerenciamento seguro do acesso aos serviços e outros recursos da AWS por meio da criação de grupo de usuário, usuários e permissões.

<div align="center">
  <img src="https://user-images.githubusercontent.com/72712095/227651287-bb0f47cf-106b-4b27-be56-f954afef6bbb.png">
</div>


<details><summary> <h3>Recursos</h3></summary>
<ul>
    <li><b>Acesso compartilhado a contas da AWS:</b> Fornece permissões de acesso a outros usuários</li>
    <li><b>Permissões granulares:</b> Usuários podem ter níveis de acessos diferentes de acordo com suas funções (papéis) em uma consta AWS</li>
    <li><b>MFA:</b> Autenticação de múltiplos fatores</li>
    <li><b>Integração com serviços AWS:</b>Estabelece níveis de permissões de acesso aos serviços AWS</li>
    <li><b>Gratuito:</b> O IAM não possui custos ou limites de uso</li>
</ul> 
</details>


<details><summary> <h3>Termos e conceitos</h3></summary>
<ul>
<li><b>Identity:</b> Fornece acesso a uma conta na AWS</li>
<li><b>IAM Users:</b> Representa uma pessoa/entidade ou serviço que utiliza serviços AWS</li>
<li><b>IAM Groups:</b> Coleção de entidades/usuários IAM
<li><b>IAM Roles:</b> Conjunto de permissões que determinam o nível de acesso de uma identidade aos serviços da AWS

<div align="center">
<img src="https://cloudiofy.com/wp-content/uploads/2022/08/iam-entities.png" width="70%">
</div>  
  
</li>
  
<li><b>IAM Policies:</b> Define permissões de acesso a serviços AWS (é um objeto) que, quando associada a um grupo e/ou a um usuário, define suas permissões. O IAM Roles (papel/função) tem em si polices. Formas de utilizar a police: 
  
<ul>
<li><b>Inline policy:</b> permissões atreladas diretamente a uma identidade (não são reaproveitáveis)
  
<div align="center">
<img src="https://docs.aws.amazon.com/pt_br/IAM/latest/UserGuide/images/policies-inline-policies.diagram.png" width="70%">
</div>

</li>
<li><b>Managed policy:</b> Conjunto de permissões disponível para várias identidades</li>
<div align="center">
<img src="https://docs.aws.amazon.com/pt_br/IAM/latest/UserGuide/images/policies-aws-managed-policies.diagram.png" width="70%">
</div>
</ul>   
</li>
<li><b>IAM Permissions:</b> Nível mais baixo da hierarquia, determina se uma identidade pode ou não tomar uma ação sobre um recurso na AWS (Allow/Deny)</li>
<li><b>Ferramentas de Segurança IAM:</b>
<ul>
  <li>Relatório de Credenciais IAM (nível de conta)
      <ul>
        <li>Um relatório que lista todos os usuários da sua conta e o status de suas diversas credenciais.</li>
      </ul>
  </li> 
  <li>Orientador de Acesso IAM (nível de usuário)
      <ul>
        <li>O Orientador de Acesso mostra as permissões de serviço concedidas a um usuário e quando esses serviços foram acessados pela última vez.</li>
        <li>Você pode usar essas informações para revisar suas políticas.</li>
      </ul>
  </li> 
</ul>

</ul>
</details>


<details><summary> <h3>Boas práticas</h3></summary>

 <p>
    A AWS tem uma lista de melhores práticas para ajudar desenvolvedores e profissionais de TI a gerenciar o acesso aos recursos da AWS.  
 </p>

<ul>
    <li><b>Conta raiz:</b> não utilizá-la em tarefas diárias de desenvolvimento. É mais voltada para gerenciar:
    <ul>
      <li>Painel de contas</li>
      <li>Definir quem são os administradores</li>
      <li>Planos e/ou serviços da AWS</li>
    </ul>
    </li>
    <li><b>Usários:</b> Crie usuários individuais e se necessário defina grupo para esses usuários</li>
    <li><b>Privilégios mínimos:</b> Prover apenas o nível de acesso necessário</li>
    <li><b>Permissões:</b> Utilizar grupos de usuários com permissões</li>
    <li><b>Auditoria:</b> Ativar o AWS CloudTrail</li>
    <li><b>Senhas:</b> Sempre use senhas fortes</li>
    <li><b>MFA:</b> Ativar para usuários privilegiados</li>
</ul> 
</details>

<details><summary><h3>Vídeo</h3></summary>
  <div align="center">
    <a href="https://www.youtube.com/watch?v=spUlvo0HNFQ" target="_blank">
        <img width="640" height="360" src="https://i.ytimg.com/vi/spUlvo0HNFQ/hq720.jpg?sqp=-oaymwEnCNAFEJQDSFryq4qpAxkIARUAAIhCGAHYAQHiAQoIGBACGAY4AUAB&rs=AOn4CLB446oCBzzCoxNAn6c-9m9LbJj4JA" alt="Watch Video" />
    </a>
  </div>
</details>
