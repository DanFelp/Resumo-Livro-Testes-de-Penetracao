# Capítulo 01 - Configurando o Laboratório Virtual

O livro pede para instalar a VMware e ensina o passo a passo para a instalação. Como o livro é mais antigo, essa parte está desatualizada, mas é fácil encontrar guias de como instalar o VMware.

Após a instalação do VMware, o livro ensina a fazer a instalação do Kali Linux. Mesma coisa, como o livro é antigo, essa parte está desatualizada, mas no próprio site oficial é possível encontrar um guia de como instalar o Kali.

## Configurando a rede de sua máquina virtual.

Como será utilizado o Kali para atacar sistemas-alvo por meio da rede, as máquinas virtuais devem estar na mesma rede virtual. O VMware oferece três opções para conexões de redes virtuais:

- **Bridge**: Conecta a rede virtual diretamente à rede local usando a mesma conexão usada pelo sistema host. A máquina virtual será somente outro nó da rede, com o próprio endereço IP.
  
- **NAT**: Também chamado de tradução de endereço de rede, define uma rede privada no computador host. A rede privada faz a tradução do tráfego de saída da máquina virtual para a rede local. Na rede local, o tráfego da máquina virtual parecerá vir do endereço IP do computador host.
  
- **Rede somente Host**: Limita a máquina virtual a uma rede privada local no host. Pode se comunicar com outras máquinas virtuais na rede somente de hosts, bem como o próprio computador host, mas não pode enviar nem receber qualquer tráfego na rede.
