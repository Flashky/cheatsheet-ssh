# cheatsheet-ssh


**Check ssh version**

```
ssh -v localhost
```

## Disable host key check

**Via command**

```
ssh -oStrictHostKeyChecking=no
```

**Using config file**

```
Host <ip>
  StrictHostKeyChecking no
```

## Autoaccept host key

*Requires OpenSSH 7.6 or higher.*

**Command**

```
ssh -oStrictHostKeyChecking=accept-new
```

**Using config file**

```
Host <ip>
  StrictHostKeyChecking accept-new
```
