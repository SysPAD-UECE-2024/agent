# SysPAD Monitor Agent - v1.2.0

O Agent de Monitoramento de Banco de Dados é uma aplicação desenvolvida em Flask (framework web Python) para registrar operações de inserção, atualização e exclusão de dados em bancos de dados protegidos. Integra-se ao ecossistema SysPAD para auditoria de conformidade com LGPD/GDPR.

# Estrutura do readme.md

Este documento está organizado nas seguintes seções principais:

1. **Funcionalidades-Chave**  
   Principais capacidades técnicas do sistema

2. **Documentação Técnica**  
   Detalhes de endpoints e especificação OpenAPI

3. **Tecnologias Utilizadas**  
   Stack tecnológico completo do back-end

4. **Instalação**  
   Guia completo para implantação (Docker e manual)

5. **Configuração de Ambiente**  
   Variáveis necessárias e pré-requisitos

6. **Usuários de Teste**  
   Credenciais pré-configuradas para validação

7. **Estrutura do Repositório**  
   Organização de diretórios e arquivos-chave

8. **Contribuição**  
   Diretrizes para colaboração no projeto

9. **Licença**  
   Direitos de uso e informações legais

# Dependências 
Tecnologias Utilizadas
Componente	Versão	Finalidade
Python	3.10+	Lógica principal do sistema
Flask	2.3.x	Framework web para APIs
SQLAlchemy	2.0.23	ORM para operações de banco
Cryptography	41.0.3	Implementação de criptografia
Flask-SQLAlchemy	3.0.3	Integração com bancos de dados
Swagger UI	4.19.0	Documentação interativa de APIs

# Instalação
Método 1: Instalação Manual
``` bash
Copy
git clone https://github.com/FRIDA-LACNIC-UECE/agent.git
cd agent

python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

# Configurar variáveis
export FLASK_APP=application.py
export API_URL="http://localhost:5000"

# Iniciar serviço
flask run --port=3000

```

Método 2: Via Docker
```bash
Copy
docker compose up --build
```

# Variáveis necessárias no .env
## Usuários de Teste

| Perfil        | Email                   | Senha         | Acessos               |
|---------------|-------------------------|---------------|-----------------------|
| Administrador | admin@example.com       | Admin@123     | Controle completo     |
| Convidado      | convidado@example.com   | Convidado@123 | Operações limitadas   |

# Licença
Este projeto não possui licença específica, podendo ser utilizado livremente para fins acadêmicos e de pesquisa. Para uso comercial, entre em contato com LARCES/UECE.
