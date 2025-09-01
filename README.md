# Documentação do Projeto

### Introdução

Este arquivo README serve como guia para instalação e execução do projeto. Ele fornece instruções detalhadas sobre como clonar o repositório Git, instalar as dependências e executar a aplicação.

## Pré-requisitos

Para seguir este guia, você precisará ter os seguintes softwares instalados em seu sistema:

1. `Git`
2. `Node.js`
3. `npm` (geralmente incluído com o Node.js)

## Instalação

1. **Clone o repositório Git:**

```
git clone https://github.com/PrimeCode-Solutions/healthfirst-fullstack.git
```

2. **Instale as dependências:**

```
npm install
```
## Execução

Para executar o projeto, utilize o seguinte comando:

```
npm run dev
```
Acesse http://localhost:3000/ para ver o projeto localmente.

É isso, está tudo pronto!

## API de Ebooks - Documentação

### Endpoints Implementados

#### Categorias
- `GET /api/ebook-categories` - Listar categorias (público)
- `POST /api/ebook-categories` - Criar categoria (admin)
- `PUT /api/ebook-categories/[id]` - Editar categoria (admin)
- `DELETE /api/ebook-categories/[id]` - Deletar categoria (admin)

#### Ebooks
- `GET /api/ebooks` - Listar ebooks com filtros
- `POST /api/ebooks` - Criar ebook (admin)
- `GET /api/ebooks/[id]` - Detalhes do ebook
- `PUT /api/ebooks/[id]` - Editar ebook (admin)
- `DELETE /api/ebooks/[id]` - Deletar ebook (admin)

#### Downloads e Acesso
- `GET /api/ebooks/[id]/download` - Download com verificação premium
- `POST /api/ebooks/[id]/access` - Registrar acesso
- `GET /api/user/ebooks` - Ebooks do usuário

#### Estatísticas
- `GET /api/ebooks/stats` - Estatísticas (admin)

### Autenticação
- Login: `admin@healthfirst.com` / `admin123`
- Middleware de autenticação implementado
- Verificação de roles (ADMIN/USER)

### Teste da API
Execute `GET /api/test-ebooks` para criar dados de teste.
