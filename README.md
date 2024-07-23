# ActiveMQ

### Instalar o ActiveMQ no Kubernetes:

- `git clone git@github.com:diegofnunesbr/activemq.git`
- `cd activemq`
- `helm install --create-namespace activemq -n activemq .`

### Configurar o ActiveMQ no arquivo hosts do Windows:

- `sudo tee -a /mnt/c/Windows/System32/drivers/etc/hosts <<< "$(ifconfig eth0 | grep 'inet ' | awk '{print $2}') activemq.local"`

### Remover o ActiveMQ no Kubernetes:

- `helm uninstall activemq -n activemq`
