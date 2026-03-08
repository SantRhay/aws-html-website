# AWS HTML Website

Projeto simples de website HTML hospedado em uma instância AWS EC2 utilizando Nginx como servidor web.

Este projeto faz parte do meu aprendizado em Cloud Computing e DevOps.

---

# Objetivo do Projeto

Criar e publicar um site HTML simples dentro de uma instância AWS EC2 utilizando um servidor Nginx.

O objetivo é aprender na prática:

- Linux
- AWS EC2
- Nginx
- HTML
- Git
- GitHub
- Deploy manual de aplicações

---

# Arquitetura do Projeto

Usuário
↓
Internet
↓
AWS EC2
↓
Nginx Web Server
↓
HTML Website

---

# Tecnologias Utilizadas

- HTML5
- Linux (Amazon Linux)
- AWS EC2
- Nginx
- Git
- GitHub

---

# Estrutura do Projeto


projeto-html-01
│
├── index.html
└── README.md


---

# Como Executar o Projeto

### 1 - Criar uma instância EC2 na AWS

Criar uma instância Linux (Amazon Linux) dentro da AWS.

---

### 2 - Conectar na instância via SSH


ssh -i chave.pem ec2-user@IP-DA-EC2


---

### 3 - Atualizar o sistema


sudo yum update -y


---

### 4 - Instalar o servidor Nginx


sudo amazon-linux-extras install nginx1 -y


---

### 5 - Iniciar o servidor


sudo systemctl start nginx


Verificar se o serviço está rodando:


sudo systemctl status nginx


---

### 6 - Criar o site HTML

Criar arquivo:


nano index.html


Conteúdo do arquivo:


<!DOCTYPE html>
<html>

<head>
<title>Meu primeiro site na AWS</title>
</head>

<body>

<h1>Projeto Web rodando na AWS</h1>

<p>Este site foi criado dentro de uma instância EC2.</p>

<p>Estudando desenvolvimento web e DevOps.</p>

</body>

</html>


---

### 7 - Publicar o site no Nginx


sudo cp index.html /usr/share/nginx/html/


---

### 8 - Acessar o site

Abrir no navegador:


http://32.192.254.167


---

# Resultado

O site HTML será exibido no navegador através do servidor Nginx rodando dentro da instância AWS EC2.

---

# Aprendizados

Neste projeto foram utilizados conceitos importantes:

- Deploy manual de aplicações
- Configuração de servidor web
- Gerenciamento de arquivos no Linux
- Versionamento de código com Git
- Publicação de projetos no GitHub

---

# Próximos Projetos

Este projeto faz parte de uma trilha de aprendizado em DevOps.

Próximos projetos planejados:

- Website HTML + CSS
- Website com Docker
- CI/CD com GitHub Actions
- Infraestrutura com Terraform
- Deploy com Kubernetes

---

# Autor
Rayane Santana

Projeto desenvolvido para estudos em Cloud Computing e DevOps.
