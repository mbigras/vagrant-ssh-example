# Vagrant SSH Exampl

> Neat trick passing vagrant ssh-config output into ssh command

## Usage

```
vagrant ssh-config > $ssh_config

ssh -F $ssh_config default sudo bash <<EOF
	apt-get update -y
	apt-get install -y nginx
EOF
```

## Links

* https://stackoverflow.com/a/23685489/2909897