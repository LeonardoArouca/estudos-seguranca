# Linux Unhatched — Cisco Networking Academy

**Plataforma:** Cisco Networking Academy  
**Certificado:** Linux Unhatched  
**Data de conclusão:** Abril/2025  

---

## O que é esse curso

Introdução prática ao terminal Linux. Cobre os comandos essenciais para navegar pelo sistema, manipular arquivos, entender permissões e executar tarefas básicas de administração.

---

## Comandos aprendidos

### Navegação

```bash
pwd                  # mostra o diretório atual (print working directory)
ls                   # lista arquivos e pastas
ls -l                # lista com detalhes (permissões, tamanho, data)
ls -a                # mostra arquivos ocultos (começam com .)
cd pasta/            # entra em uma pasta
cd ..                # volta uma pasta
cd ~                 # vai para o diretório home
```

### Manipulação de arquivos

```bash
cp origem destino    # copia arquivo
mv origem destino    # move ou renomeia arquivo
rm arquivo           # remove arquivo
rm -r pasta/         # remove pasta e conteúdo
mkdir pasta          # cria pasta
touch arquivo.txt    # cria arquivo vazio
cat arquivo.txt      # exibe conteúdo do arquivo
```

### Permissões

```bash
chmod 755 arquivo    # muda permissões (numérico)
chmod +x arquivo     # adiciona permissão de execução
chown user arquivo   # muda dono do arquivo
```

#### Como ler permissões no `ls -l`

```
-rw-r--r--  1  sysadmin  sysadmin  647  Dec 20 2017  hello.sh
│└────────┘  │  └──────┘  └──────┘  │    └─────────┘  └──────┘
│ permissões │   dono      grupo   tamanho   data       nome
│
└─ tipo: - arquivo | d diretório | l link
```

As 9 letras de permissão são 3 grupos de 3:

| Grupo | Letras | Significado |
|-------|--------|-------------|
| Dono | `rw-` | lê e escreve, não executa |
| Grupo | `r--` | só lê |
| Outros | `r--` | só lê |

Letras possíveis: `r` (ler), `w` (escrever), `x` (executar), `-` (sem permissão)

### Visualização de conteúdo

```bash
cat arquivo          # mostra tudo de uma vez
more arquivo         # mostra página por página
head arquivo         # mostra primeiras 10 linhas
tail arquivo         # mostra últimas 10 linhas
tail -f arquivo      # mostra em tempo real (útil para logs)
```

### Informações do sistema

```bash
whoami               # mostra usuário atual
hostname             # mostra nome da máquina
uname -a             # informações do sistema operacional
df -h                # espaço em disco
free -h              # memória RAM disponível
ps                   # processos em execução
```

---

## Conceitos importantes

### Estrutura de diretórios do Linux

```
/                    # raiz do sistema
├── home/            # pastas dos usuários
├── etc/             # arquivos de configuração
├── var/             # logs e dados variáveis
├── tmp/             # arquivos temporários
├── bin/             # comandos essenciais
└── usr/             # programas instalados
```

### Por que Linux importa em cibersegurança

- Servidores corporativos rodam Linux
- Ferramentas de pentest (Kali Linux, Nmap, Metasploit) rodam em Linux
- Análise de logs e resposta a incidentes acontece no terminal
- SOC, Blue Team e Red Team usam Linux no dia a dia

---

## Próximo passo

**Linux Essentials** — Cisco Networking Academy (certificado mais completo)
