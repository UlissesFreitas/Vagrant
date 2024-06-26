
# Notas de estudo sobre infra as a code com vagrant



Inicialização do projeto e alteração do vagrantfile, especificado o provider e as configurações da VM como memoria, CPUs e o nome da VM


## Vagrantfile

Dizendo qual imagem iremos usar na VM
```bash
  config.vm.box = "centos/7"
```

Selecionando o provider e as configurações da VM

```bash
  config.vm.provider "hyperv" do |h|
    h.memory = "1024"
    h.vmname = "Centos-02"
    h.cpus = 2
  end

```
## Comandos

Para criar/iniciar a VM com o vagrant

```bash
  vagrant init 
```

Subir a VM
```bash
  vagrant up
```

Desligar a VM
```bash
  vagrant halt
```

Acessar a VM
```bash
  vagrant ssh
```

Destruir a VM
```bash
  vagrant destroy
```