# **Startup Investment Platform** 🌟

Uma plataforma desenvolvida em **Django** para conectar empreendedores e investidores, permitindo a criação de propostas de investimento, gerenciamento de empresas e documentos, além de uma interface moderna para visualização de métricas e progresso.

## **🚀 Funcionalidades**

1. **Cadastro e Login de Usuários**
   - Sistema de autenticação para acesso às funcionalidades principais.

2. **Empresas**
   - Cadastro de empresas com detalhes como nome, CNPJ, estágio, área de atuação, pitch e logo.
   - Gerenciamento de documentos e métricas da empresa.
   - Exibição de informações detalhadas sobre o status da captação de recursos.

3. **Investidores**
   - Listagem de empresas disponíveis para investimento com filtros personalizados.
   - Envio de propostas de investimento, incluindo valor e percentual de equity.
   - Acompanhamento do progresso das propostas enviadas e gestão do contrato.

4. **Métricas Dinâmicas**
   - Cálculo do valuation atual e percentual captado com base nas propostas aceitas.
   - Registro de métricas adicionais personalizadas por empresa.

5. **Documentos**
   - Upload e exclusão de documentos no formato PDF.
   - Organização dos documentos para cada empresa.

## **📂 Estrutura do Projeto**

O projeto está dividido em três principais aplicativos Django:

1. **Usuários (`usuarios`)**
   - Gerencia o cadastro e login de usuários.

2. **Empresários (`empresarios`)**
   - Gerencia o cadastro e listagem de empresas, incluindo o upload de documentos e registro de métricas.

3. **Investidores (`investidores`)**
   - Facilita a busca por empresas, envio de propostas de investimento e gerenciamento de contratos.

## **🔧 Configuração do Ambiente**

### **Pré-requisitos**

Certifique-se de ter o **Python 3.8+** e o **Django 4.x** instalados.

### **Instalação**

1. Clone o repositório:
   ```bash
   git clone https://github.com/Alisonsantos77/psw11.git
   cd psw11
   ```

2. Crie um ambiente virtual:
   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows: venv\Scripts\activate
   ```

3. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

4. Configure o banco de dados:
   - Edite o arquivo `settings.py` para ajustar as configurações do banco de dados conforme necessário (SQLite, PostgreSQL, etc.).
   - Aplique as migrations:
     ```bash
     python manage.py migrate
     ```

5. Crie um superusuário para acessar o admin:
   ```bash
   python manage.py createsuperuser
   ```

6. Inicie o servidor de desenvolvimento:
   ```bash
   python manage.py runserver
   ```

7. Acesse o aplicativo no navegador:
   - [http://localhost:8000](http://localhost:8000)

### **Arquivos Estáticos**
Certifique-se de coletar os arquivos estáticos para produção:
```bash
python manage.py collectstatic
```

## **🌟 Funcionalidades por Página**

1. **Cadastro de Empresas**
   - Página para que empresários possam cadastrar detalhes completos de suas startups.
   - Upload de pitch e logo para apresentação.

2. **Listagem de Empresas**
   - Filtro para buscar empresas específicas.
   - Exibição de progresso da captação com barra de progresso.

3. **Detalhes da Empresa**
   - Informações completas sobre o progresso da captação.
   - Métricas e documentos da empresa.

4. **Propostas de Investimento**
   - Página para investidores enviarem propostas.
   - Opções de aceitação ou recusa de propostas pelo empresário.

## **📚 Créditos e Autor**

**Desenvolvido por:** Alison Santos  
Perfil do LinkedIn: [Alison Santos](https://www.linkedin.com/in/alisonsantosdev)  
GitHub: [Alisonsantos77](https://github.com/Alisonsantos77)

## **📜 Licença**

Este projeto está licenciado sob a licença **MIT**. Consulte o arquivo `LICENSE` para mais detalhes.
