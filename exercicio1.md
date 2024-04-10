1. Atualização do sistema:

Utilizei o comando sudo apt update && sudo apt upgrade para atualizar o sistema operacional Ubuntu Server. A atualização foi realizada sem problemas, garantindo que todos os pacotes e o kernel estejam na versão mais recente.
2. Edição do arquivo de configuração system.conf:

Acessei o arquivo de configuração system.conf localizado em /etc/sysctl.d/ utilizando o editor de texto Nano.
Adicionei a linha vm.swappiness=10 ao arquivo para definir o parâmetro vm.swappiness com um valor de 10, priorizando o uso da memória RAM física em detrimento da troca de memória para o disco.
Consultei o arquivo README.md para entender o impacto do parâmetro vm.swappiness e documentei essa informação para referência futura.
3. Verificação da alocação de recursos:

Utilizei os comandos top e htop para monitorar o uso de recursos como memória e CPU.
Identifiquei e tomei nota de quaisquer processos que estavam consumindo uma quantidade excessiva de recursos para investigação adicional.
4. Ajuste das definições de CPU e RAM na aplicação VirtualBox:

Acessei as configurações da máquina virtual Ubuntu Server na interface gráfica do VirtualBox.
Aumentei ligeiramente a alocação de RAM e CPU para melhorar o desempenho do servidor.
Documentei os valores antes e depois do ajuste, observando como valores mais altos impactam positivamente o desempenho da máquina virtual, mas também podem afetar o desempenho do host se os recursos físicos forem compartilhados.
