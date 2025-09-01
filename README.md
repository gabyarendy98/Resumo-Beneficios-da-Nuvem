# Resumo-Beneficios-da-Nuvem
Resumo Beneficios da Nuvem

📌 Resumo – Criar Máquina Virtual Windows no Azure (Portal)

Entrar no Azure

Acesse o [Portal do Azure].

Pesquise por Máquinas Virtuais → Criar → Máquina Virtual do Azure.

Configuração da VM

Nome: myVM.

Imagem: Windows Server 2022 Datacenter.

Usuário administrador: ex. azureuser.

Senha: mínimo 12 caracteres.

Regras de porta: habilitar RDP (3389) e HTTP (80).

Implantação

Clique em Examinar + Criar → Criar.

Após a validação, acesse o recurso criado.

Conexão via RDP

Na VM, selecione Conectar > RDP.

Baixe o arquivo RDP, abra e entre com usuário/senha definidos.

Instalar Servidor Web IIS

No PowerShell da VM, execute:

Install-WindowsFeature -name Web-Server -IncludeManagementTools


Depois, acesse o IP público da VM no navegador → página padrão do IIS será exibida.

Gerenciamento e Limpeza

Para não gerar custos: excluir o grupo de recursos ou habilitar desligamento automático da VM.
