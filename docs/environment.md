# 環境設定 

## vagrant(on local machine)

```bash
mkdir -p ~/Boxes/node && cd $_
vagrant init ubuntu/focal64
```

edit Vagrantfile

```
26: config.vm.network "forwarded_port", guest: 3000, host: 3000

52: config.vm.provider "virtualbox" do |vb|
53:  #   # Display the VirtualBox GUI when booting the machine
54:  #   vb.gui = true
55:  #
56:  #   # Customize the amount of memory on the VM:
57:     vb.memory = "2048"
58: end
```

```bash
vagrant up
vagrant ssh
```

## node install(on vagrant machine)

```sh
sudo apt update -y
sudo apt install nodejs npm
sudo npm install -g n
sudo n lts
sudo apt purge nodejs npm
sudo apt autoremove
sudo npm install -g npm
sudo npm install -g yarn
```

## standardjs and jest

```sh
sudo npm install -g standard
sudo npm install -g jest
```

## vscode plugin and module install

```code```

- `ctrl + P` -> `ext install VisualStudioExptTeam.vscodeintellicode`
- `ctrl + P` -> `ext install standard.vscode-standard`
- `ctrl + P` -> `ext install capaj.vscode-standardjs-snippets`
- `ctrl + P` -> `ext install firsttris.vscode-jest-runner`

## snippets

snippets -> see [document](../snippet/README.md)
