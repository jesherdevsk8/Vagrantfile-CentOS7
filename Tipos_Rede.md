## TIPOS DE REDE NO VAGRANT

### __Resumo:__
**Existem 3 formas para configurar a rede:**

- Forwarded Port
- Private Network
- Public Network

Na configuração **Forwarded Port**, mapeamos uma porta do host para o guest, por exemplo:
config.vm.network “forwarded_port”, guest: 80, host: 8080,

Na **Private Network (static ou dhcp)** é usado um endereço privado que não é acessível na sua rede pública (por exemplo, a rede empresarial)

Na **Public Network (static ou dhcp)**, usamos um endereço que faz parte da sua rede pública (por exemplo, da rede empresarial)

Com o comando vagrant halt podemos parar a execução da máquina virtual

O comando vagrant reload recarrega a configuração da máquina virtual
