# SilvioISO – Ferramenta de Criação de ISOs Personalizadas

Se você é usuário do **SilvioLinux**, deve **provar a ferramenta SilvioISO** e criar a **sua própria distribuição Linux baseada no SilvioLinux**.

O **SilvioLinux** é uma distribuição criada por **Sílvio Ramalho Neto da Silva**, baseada no **Yocto Project** e que utiliza o **gerenciador de pacotes `opkg`**. Para facilitar a criação de ISOs personalizadas, o autor lançou a ferramenta **SilvioISO**, escrita em **Shell Script** e **Python3** e **GTK-4.0**.

> ⚠️ **Importante:** A ferramenta **SilvioISO só é suportada no SilvioLinux**. É necessário ter o **SilvioLinux instalado no computador** para utilizar esta ferramenta.

---

## 📦 O que é o SilvioISO?

O **SilvioISO** é uma ferramenta oficial para criação de **ISOs customizadas** do SilvioLinux, permitindo que você gere sua própria distribuição derivada, com pacotes, configurações e personalizações específicas.

---

## 🛠️ Requisitos

- SilvioLinux instalado no sistema
- Arquitetura suportada:
  - **32 bits (i686)**
  - **64 bits (x86_64)**
- Gerenciador de pacotes: `opkg`

---

## 🔄 Atualização do Sistema

Antes de instalar o SilvioISO, **atualize o sistema**:

```bash
sudo opkg update
sudo opkg upgrade
```

---

## 📥 Instalação do SilvioISO

Instale a ferramenta utilizando o `opkg`:

```bash
sudo opkg install silvioiso
```

Durante a instalação, o SilvioISO irá instalar automaticamente as **dependências necessárias**, incluindo:

- `build-essential`
- `python3`
- `gtk-4.0-devel`

---

## 📄 Arquivos Obrigatórios (.silvioisospec)

Para que a criação da ISO funcione corretamente, **é obrigatório possuir um dos arquivos abaixo**, de acordo com a arquitetura do sistema:

- **32 bits:**
  ```
  SilvioLinux-i686-20280316.silvioisospec
  ```

- **64 bits:**
  ```
  SilvioLinux-x86_64-20280316.silvioisospec
  ```

Esses arquivos definem as especificações da ISO a ser gerada.

---

## 📁 Estrutura de Pastas (Obrigatória)

O SilvioISO utiliza pastas **ocultas** (com ponto `.` no início). Elas são criadas automaticamente, mas é importante conhecer sua função:

- Pasta de build (obrigatória):
  ```
  ~/.silvioiso/build/
  ```

- Pasta onde a ISO final será gerada:
  ```
  ~/.silvioiso/tmp/images/iso/
  ```

> ⚠️ **Não altere nem remova essas pastas**, pois elas são essenciais para o processo de compilação.

---

## ⚙️ Gerando a ISO

Para gerar sua ISO personalizada, utilize o comando:

```bash
mksilvioiso -s
```

Após o processo de compilação, a **ISO final** estará disponível em:

```bash
~/.silvioiso/tmp/images/iso/
```

---

## 🚀 Crie Sua Própria Distribuição

Com o **SilvioISO**, você pode:

- Criar uma distribuição Linux personalizada
- Gerar ISOs próprias baseadas no SilvioLinux
- Adaptar o sistema para hardware específico
- Criar versões minimalistas ou completas

Se você é usuário do SilvioLinux, **experimente o SilvioISO e crie sua própria distro!**

---

## 👤 Autor

**Sílvio Ramalho Neto da Silva**  
Criador do SilvioLinux e da ferramenta SilvioISO

---

## 📜 Licença

Consulte o arquivo `LICENSE` para mais informações sobre a licença do projeto.
