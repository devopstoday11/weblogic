# weblogic

deploying an Oracle WebLogic Server application Two-cluster architecture and administrative server using terraform and Ansible

## Подготовка к установке для развёртывания инфраструктуры

Компания Hashicorp <https://www.hashicorp.com/> поставляет на рынок opensource решения, направленые на решение задач управления инфраструктурой.

- Vault - позволяет управлять секретами.
- Terraform - позволяет создавать и отслеживать инфраструктуру.Отличительной особенностью является наличие файла блокирующего одновременное изменение инфраструктуры несколькими пользователями.

Terraform представляет мобой модульное решение, позволяющее использовать различные облачные решения <https://www.terraform.io/docs/providers/index.html>. </br>
Для исользования Qemu виртуализации, требуется описать провайдер или использовать <https://github.com/dmacvicar/terraform-provider-libvirt>

### Jolokia

<https://jolokia.org/index.html> Мониторинг WebLogic сервера

### Start WebLogic Managed Server Commans Line

<pre><code>
cd $DOMAIN_HOME/bin

nohup ./startManagedWebLogic.sh [InstanceName] [t3 Admin URL] > $DOMAIN_HOME/servers/[InstanceName]/[InstanceName].out 2>&1 &
</code></pre>
