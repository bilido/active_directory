# 01 Installing Domain Controller

1. Use `sconfig` to:
    - Change the hostname
    - Change the IP address to static
    - Change the DNS server to our own IP address

2. Install the Active Directory Windows Feature

```shell
Install-WindowsFeature -name AD-Domain-Services -IncludeManagementTools
```

```shell
Get-NetIPAddress
```

# Joining the workstation to the domain


```
Add-Computer -DomainName xyz.com -Credential xyz\Administrator -Force -Restart
```


