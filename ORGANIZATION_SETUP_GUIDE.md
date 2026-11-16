# 📋 Guia de Configuração: Perfil da Organização GitHub

Este guia contém as orientações exatas para ativar a descrição e a vitrine oficial da organização **TODOS-Empreendimentos** no GitHub.

---

## 1. Configurar Metadados no Painel do GitHub

Acesse a página da organização e vá em:
👉 **Settings** (da Organização) ➔ **General** ➔ **Organization profile**

Preencha os campos exatamente assim:

| Campo | Valor Recomendado |
| :--- | :--- |
| **Organization display name** | `TEC TODOS` *(ou `TEC TODOS \| TODOS Empreendimentos`)* |
| **Description** *(Opção 2 Escolhida)* | `Tecnologia, Automação e Inteligência Artificial impulsionando o maior ecossistema de saúde, educação e benefícios do Brasil.` |
| **Website URL** | `https://www.cartaodetodos.com.br` |
| **Location** | `Brasil` |
| **Public email** | *(E-mail do time de tecnologia / suporte interno)* |

Clique em **Save changes**.

---

## 2. Publicar a Vitrine (Profile README)

O GitHub exige que o Profile README de uma organização fique dentro de um repositório especial com o nome **`.github`** configurado como **Público (Public)**.

### Passo a Passo no GitHub:
1. No menu superior da organização, clique em **Repositories** ➔ **New**.
2. No campo **Repository name**, digite rigorosamente:  
   `.github`
3. Selecione a visibilidade: **Public** *(obrigatório para que o GitHub exiba para todos)*.
4. Não marque a opção de adicionar README pelo site (pois vamos enviar os arquivos deste diretório local).
5. Clique em **Create repository**.

### Passo a Passo no Terminal (a partir de `C:\Projetos\GitHub-Todos`):

Abra o terminal dentro desta pasta (`C:\Projetos\GitHub-Todos`) e execute:

```bash
# 1. Inicializar o repositório Git local
git init

# 2. Adicionar os arquivos criados
git add .

# 3. Criar o commit inicial
git commit -m "feat: setup official organization profile README and guidelines"

# 4. Definir a branch principal como main
git branch -M main

# 5. Conectar ao repositório remoto recém-criado
git remote add origin https://github.com/TODOS-Empreendimentos/.github.git

# 6. Enviar para o GitHub
git push -u origin main
```

> **Nota:** Imediatamente após o `git push`, ao acessar `https://github.com/TODOS-Empreendimentos`, a página inicial exibirá todo o banner, badges, stack e documentação da TEC TODOS.

---

## 3. Repositórios em Destaque (Pinned Repositories)

Na página inicial da organização (`https://github.com/TODOS-Empreendimentos`):
1. No canto superior direito da seção de repositórios, clique em **Customize your pins**.
2. Selecione até 6 repositórios que demonstram a força técnica do time (ex: os painéis principais, templates ou automações chave).
3. Salve as alterações.
