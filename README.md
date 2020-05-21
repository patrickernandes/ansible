# ansible

Algumas dicas e scripts para aplicação do ansible na automatização de um host Linux.

Para início, esta será a estrutura para um host:

```
host
├── files
│   └── setup8.sh
├── vars
│   └── default.yml
├── playbook.yml
└── readme.md
```

- `files/`: pasta com scripts e arquivos de configurações.
- `vars/`: pasta com as variáveis do arquivo 'default.yml'.
- `playbook.yml`: arquivo playbook.
- `readme.md`: arquivo com descriçao de apoio.

## Teste de conexão:

Através do host aonde o amsible está instalado, realizar um teste de conexão com host destino:

```
ansible all -m ping -u usuário_do_destino
```

