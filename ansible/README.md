# Automation

It is based off Ansible. 

## Vault Management

### Encrypt/Decrypt Variables

```bash
$> ansible-vault encrypt variables.yaml --vault-password-file ~/.ansible_vault_passwd
```

```bash
$> ansible-vault decrypt variables.yaml --vault-password-file ~/.ansible_vault_passwd
```

### Encrypt/Descrypt Certificates

```bash
$> ansible-vault encrypt certs.yaml --vault-password-file ~/.ansible_vault_passwd
```

```bash
$> ansible-vault decrypt certs.yaml --vault-password-file ~/.ansible_vault_passwd
```


## Playbook Run

### Basics Machine Configuration

```bash
$> ansible-playbook -i hosts configure_machines.yaml --vault-password-file ~/.ansible_vault_passwd
```

### Basics Deploy Configuration

```bash
$> ansible-playbook -i hosts configure_deploys.yaml --vault-password-file ~/.ansible_vault_passwd
```