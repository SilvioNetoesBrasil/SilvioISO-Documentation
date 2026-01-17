# SilvioISO

Se você é usuário do **SilvioLinux**, você deve **provar a ferramenta SilvioISO** e criar **sua própria distribuição Linux baseada no SilvioLinux**.

O **SilvioLinux** é uma distribuição Linux **minimalista e leve**, baseada no **Yocto Project**, utilizando o **gerenciador de pacotes opkg**. Seu criador, **Sílvio Ramalho Neto da Silva**, lançou a ferramenta **SilvioISO**, que permite a criação de **ISOs personalizadas** de forma simples e eficiente.

---

## 📦 O que é o SilvioISO?

**SilvioISO** é uma ferramenta de criação de ISOs personalizadas do SilvioLinux, **escrita em Shell Script e Lua**, projetada para ser simples, leve e eficiente.

Ela permite que qualquer usuário do SilvioLinux gere sua própria ISO customizada com poucos comandos.

---

## ⚙️ Requisitos Importantes

⚠️ **Atenção:**

- O **SilvioISO só funciona no SilvioLinux**
- É **obrigatório** ter o **SilvioLinux instalado** no seu computador
- Não há suporte para outras distribuições Linux

---

## 🔄 Atualizando o Sistema

Antes de instalar o SilvioISO, é altamente recomendado manter o sistema atualizado:

```bash
sudo opkg update
sudo opkg upgrade
```

---

## 📥 Instalação do SilvioISO

A instalação é feita diretamente pelo gerenciador de pacotes **opkg**:

```bash
sudo opkg install silvioiso
```

Durante a instalação, o SilvioISO irá instalar automaticamente todas as dependências necessárias.

### Dependências instaladas automaticamente

- build-essential
- python3
- gtk-4.0-devel

---

## 🛠️ Como Gerar Sua ISO Personalizada

Após a instalação, utilize o comando abaixo para gerar sua ISO personalizada:

```bash
mksilvioiso -s
```

Esse comando irá iniciar o processo de criação da ISO baseada no seu sistema SilvioLinux atual.

---

## 🎯 Objetivo do Projeto

O SilvioISO foi criado para:

- Facilitar a criação de distribuições personalizadas
- Incentivar usuários a criarem seus próprios sistemas
- Manter a filosofia **leve, minimalista e eficiente** do SilvioLinux

Se você usa o SilvioLinux, **crie, personalize e distribua sua própria ISO** 🚀

---

## 👤 Autor

**Sílvio Ramalho Neto da Silva**  
Criador do SilvioLinux e da ferramenta SilvioISO

---

## 📜 Licença

Consulte o arquivo **LICENCE.txt** para mais informações sobre a licença do projeto.
