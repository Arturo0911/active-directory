# Active Directory


## Objects:

  - Users: User accounts contain information about yusres, including the information required to authenticate a user during the singnin process and build the user's access token.
  - Computers: Each domain-joined computer has an account in AD DS. You can use computer accounts for domain-joined computers in the same way that you use user accounts for users.
  - Groups: Groups organize users or computers to simplify the management of permissions and Groups Policy Objects in the domain.



Get-EventLog Command

```bash
Get-EventLog -LogName <Event Type (Application, System, Securiry)> -Newest <number of recent rows> | Format-List -Property *
```

Adding Users with cmd

```bash
net user hackthur hackthur123$! /add

net localgroup Administrators hackthur /add

net localgroup "Remote Desktop Users" hackthur /ADD
```




To eliminate a task you should to use this command


```bash
sc queryex <process name>
# to eliminate
taskkill /f /pid <pid number>
```
