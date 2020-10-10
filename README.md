# metasploit-behind-ssl
Running C2 on Metasploit @AWS behind NginX SSL connection provided by Let's Encrypt


## CloudFormation
Kali Linux up and running:

```
aws cloudformation create-stack --stack-name metasploit --template-body file://cfn/metasploit.yml --parameters file://cfn/metasploit.params.json
```

## Ansible



## Vagrant

Download Windows image from 

```
https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/
```

Unzip and add image to vagrant

```
vagrant box add MsEdge\ -\ Win10.box --name windows10
```

Ensure you have WinRM plugins and run vagrant
```
vagrant plugin install winrm
vagrant plugin install winrm-fs
vagrant plugin install winrm-elevated

vagrant up
```
