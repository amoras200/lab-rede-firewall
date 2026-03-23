# 🔐 Laboratório de Redes e Firewall com Linux

Projeto prático de virtualização, redes e segurança em Linux. Criação de duas máquinas virtuais (KVM) com Ubuntu Server, configuração de rede interna isolada, IPs estáticos, firewall com iptables e escaneamento de rede com nmap.

---

## 📌 Objetivo

Demonstrar conhecimentos em:
- Virtualização com KVM/virt-manager
- Configuração de redes internas
- IPs estáticos com netplan
- Firewall com iptables
- Escaneamento de rede com nmap

---

## 🧱 Tecnologias utilizadas

| Ferramenta              | Finalidade                  |
| ----------------------- | --------------------------- |
| **KVM + virt-manager**  | Virtualização das máquinas  |
| **Ubuntu Server 24.04** | Sistema operacional das VMs |
| **Netplan**             | Configuração de redes       |
| **iptables**            | Firewall                    |
| **nmap**                | Escaneamento de rede        |

---

## 📦 Passo a passo

### 1. Criar as VMs no KVM

Duas VMs com Ubuntu Server:
- **VM1:** 1GB RAM, 10GB disco, nome `VM1-Seguranca`
- **VM2:** 1GB RAM, 10GB disco, nome `VM2-Seguranca`

![Criação das VMs](prints/criando-vms.png)

---

### 2. Instalar Ubuntu Server

Configurações padrão:
- Usuário: `aluno`
- Senha: `aluno`
- OpenSSH Server: ✅ instalado

![Instalação do sistema](prints/logs instalação sistema.png)

![Atualizações](prints/updatesystem.png)

![Instalação completa](prints/instalacao completa.png)

---

### 3. Login e primeiro acesso

![Login na VM](prints/logcusto.png)

![Login OK](prints/logeo OK.png)

![Terminal pronto](prints/pronto.png)

---

### 4. Conectar via SSH do host

```bash
ssh aluno@192.168.122.242   # VM1
ssh aluno@192.168.122.241   # VM2