# NovaStall - Plataforma E-commerce Moderna

Bem-vindo ao NovaStall! Uma plataforma de e-commerce desenvolvida com Django e Python, apresentando um design moderno e responsivo utilizando Bootstrap 5.

## 🚀 Sobre o Projeto

O NovaStall é um sistema de loja virtual projetado para oferecer uma experiência de compra fluida e agradável. Ele permite o cadastro de produtos, gerenciamento de usuários, visualização de produtos em destaque e uma interface administrativa para controle total da loja. A identidade visual foi recentemente atualizada para um estilo contemporâneo, com foco na usabilidade e estética.

## ✨ Funcionalidades Principais

* **Listagem de Produtos:** Visualização clara e organizada dos produtos, com imagens, descrições e preços.
* **Produtos em Destaque:** Seção para exibir os produtos mais vendidos ou em promoção.
* **Design Responsivo:** Interface adaptável para uma ótima experiência em desktops, tablets e smartphones, construída com Bootstrap 5.
* **Autenticação de Usuários:** Sistema de login e cadastro de usuários.
* **Gerenciamento de Usuários:** (Para administradores) Capacidade de visualizar, adicionar, editar e excluir usuários.
* **Gerenciamento de Produtos:** (Para administradores) CRUD completo para produtos, incluindo nome, descrição, preço, imagem e estoque.
* **Painel Administrativo (Dashboard):** (Para administradores) Visualização de gráficos e informações relevantes sobre vendas e estoque (funcionalidade em desenvolvimento/a ser implementada).
* **Checkout Simplificado:** Processo de compra direto para os produtos.
* **Identidade Visual Moderna:** Utiliza a fonte "Inter", cores sofisticadas e componentes Bootstrap atualizados.

## 🛠️ Tecnologias Utilizadas

* **Backend:**
    * Python 3.x
    * Django 5.x (ou a versão que você está utilizando)
* **Frontend:**
    * HTML5
    * CSS3
    * Bootstrap 5.3
    * JavaScript (mínimo, principalmente via Bootstrap)
    * Google Fonts (Inter)
    * Font Awesome (Ícones)
* **Banco de Dados:**
    * SQLite (padrão do Django para desenvolvimento, pode ser alterado para PostgreSQL, MySQL, etc., para produção)

## ⚙️ Configuração e Instalação

Siga os passos abaixo para configurar e executar o projeto em seu ambiente local:

1.  **Clone o Repositório:**
    ```bash
    git clone <url-do-seu-repositorio-git>
    cd nome-da-pasta-do-projeto # Ex: cd NovaStall
    ```

2.  **Crie e Ative um Ambiente Virtual:**
    É altamente recomendável usar um ambiente virtual para isolar as dependências do projeto.
    ```bash
    # Windows
    python -m venv ambienteVirtual
    ambienteVirtual\Scripts\activate

    # macOS/Linux
    python3 -m venv ambienteVirtual
    source ambienteVirtual/bin/activate
    ```

3.  **Instale as Dependências:**
    Certifique-se de ter um arquivo `requirements.txt` com as dependências do projeto. Se não tiver, você pode gerá-lo com `pip freeze > requirements.txt` após instalar as bibliotecas necessárias (como Django, Pillow, etc.).
    ```bash
    pip install -r requirements.txt
    ```
    Principais dependências que você provavelmente precisará (se ainda não estiverem no `requirements.txt`):
    ```bash
    pip install Django Pillow # Pillow é para manipulação de imagens (upload de fotos de produtos)
    ```

4.  **Execute as Migrações do Banco de Dados:**
    As migrações criam as tabelas necessárias no banco de dados.
    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

5.  **Crie um Superusuário (Administrador):**
    Isso permitirá que você acesse o painel de administração do Django.
    ```bash
    python manage.py createsuperuser
    ```
    Siga as instruções para definir nome de usuário, email e senha.

6.  **Execute o Servidor de Desenvolvimento:**
    ```bash
    python manage.py runserver
    ```
    Por padrão, o servidor estará acessível em `http://127.0.0.1:8000/`.

## 📁 Estrutura do Projeto (Simplificada)


nome-da-pasta-do-projeto/
├── app/                    # Aplicativo principal da loja (views, models, templates, static, etc.)
│   ├── migrations/
│   ├── static/             # Arquivos estáticos específicos do app (CSS, JS, imagens)
│   │   └── css/
│   │       └── nova_stall_styles.css
│   ├── templates/          # Templates HTML do app
│   │   ├── template.html   # Template base
│   │   └── ... (outros templates)
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── urls.py
│   └── views.py
├── projeto/                # Configurações do projeto Django (settings.py, urls.py principal, etc.)
│   ├── init.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── ambienteVirtual/        # Pasta do ambiente virtual (não versionar)
├── manage.py               # Utilitário de linha de comando do Django
├── db.sqlite3              # Banco de dados SQLite (padrão)
└── README.md               # Este arquivo


## 🎨 Estilização e Design

* O design principal é implementado utilizando **Bootstrap 5**.
* Estilos personalizados e overrides do Bootstrap estão no arquivo `app/static/css/nova_stall_styles.css`.
* A fonte principal é **Inter**, importada do Google Fonts.
* Ícones são fornecidos pelo **Font Awesome**.

## 🤝 Como Contribuir (Exemplo)

Contribuições são bem-vindas! Se você deseja contribuir para o projeto:

1.  Faça um Fork do projeto.
2.  Crie uma branch para sua feature (`git checkout -b feature/MinhaNovaFeature`).
3.  Faça commit de suas mudanças (`git commit -m 'Adiciona MinhaNovaFeature'`).
4.  Faça push para a branch (`git push origin feature/MinhaNovaFeature`).
5.  Abra um Pull Request.

## 📝 Licença (Exemplo)

Este projeto está licenciado sob a Licença MIT. Veja o arquivo `LICENSE` para mais detalhes (se você adicionar um).

---

Feito com ❤️ e Python!
