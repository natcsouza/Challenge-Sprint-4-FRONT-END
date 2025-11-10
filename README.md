# 🏥 Hospital Clínico - Sistema de Gestão Hospitalar
 
## 📋 Sobre o Projeto
 
O Hospital Clínico é uma aplicação web moderna desenvolvida em **React + Vite + TypeScript**, focada em proporcionar uma experiência de usuário excepcional para pacientes e profissionais da saúde. O projeto foi desenvolvido como parte da **Sprint 03**, implementando rotas dinâmicas, consumo de API REST, tipos TypeScript avançados e responsividade completa.
 
## 🎯 Objetivo
 
Desenvolver uma solução inovadora para reduzir a taxa de absenteísmo hospitalar de 20% para menos de 10% através do **GUIDABOT** - uma assistente digital humanizada que atua como elo entre paciente, acompanhante e equipe médica.
 
## 🚀 Tecnologias Utilizadas
 
- **React 18** - Biblioteca para construção de interfaces
- **TypeScript** - Superset do JavaScript com tipagem estática
- **Vite** - Build tool moderna e rápida
- **React Router DOM v6** - Roteamento para SPA com rotas estáticas e dinâmicas
- **React Hook Form** - Gerenciamento de formulários
- **TailwindCSS** - Framework CSS utilitário para estilização e responsividade
- **Font Awesome** - Ícones vetoriais
 
## 👥 Equipe de Desenvolvimento
 
### 1TDSR ADS - Turma de Análise e Desenvolvimento de Sistemas
 
| Nome | RM | Função | LinkedIn | GitHub |
|------|----|---------|---------|---------|
| **Rafael Malaguti** | 561830 | Líder | [LinkedIn](https://www.linkedin.com/in/rafael-malaguti-481730340/) | [GitHub](https://github.com/rafaelmalaguti) |
| **Natalia Cristina Souza** | 564099 | Vendedora | [LinkedIn](https://www.linkedin.com/in/natalia-cristina-de-souza-333b92169) | [GitHub](https://github.com/natcsouza) |
| **Lincoln Roncato** | 565944 | Desenvolvedor | [LinkedIn](https://www.linkedin.com/in/lincoln-roncato-266233353) | [GitHub](https://github.com/lincolnroncato) |
 
## 🏗️ Estrutura do Projeto
 
```
hospital-clinico/
├── public/
│   └── images/          # Imagens dos membros da equipe
├── src/
│   ├── components/      # Componentes reutilizáveis
│   │   ├── Header.tsx
│   │   ├── Footer.tsx
│   │   ├── Card.tsx
│   │   ├── Button.tsx
│   │   ├── Hero.tsx
│   │   ├── FAQ.tsx
│   │   ├── ContactForm.tsx
│   │   ├── Toast.tsx
│   │   └── ToastContainer.tsx
│   ├── pages/           # Páginas da aplicação
│   │   ├── Home.tsx
│   │   ├── Especialidades.tsx
│   │   ├── EspecialidadeDetalhes.tsx
│   │   ├── Equipe.tsx
│   │   ├── FAQ.tsx
│   │   ├── Contato.tsx
│   │   ├── Solucao.tsx
│   │   ├── NotFound.tsx
│   │   ├── Pacientes.tsx
│   │   └── PacienteForm.tsx
│   ├── services/        # Serviços de API
│   │   └── api.ts       # Serviço de consumo da API REST
│   ├── hooks/           # Custom hooks
│   │   └── useToast.ts  # Hook para notificações
│   ├── data/            # Dados mockados
│   │   └── mockData.ts
│   ├── types/           # Definições de tipos TypeScript
│   │   └── index.ts     # Tipos básicos, Union Types, Intersection Types e Interfaces
│   ├── App.tsx          # Componente principal com rotas
│   ├── main.tsx         # Ponto de entrada
│   └── index.css        # Estilos globais
├── .env.example         # Exemplo de variáveis de ambiente
├── tailwind.config.js   # Configuração do TailwindCSS
├── postcss.config.js    # Configuração do PostCSS
├── vite.config.ts       # Configuração do Vite
└── package.json         # Dependências do projeto
```
 
## 🎨 Design System
 
### Cores
- **Hospital Blue**: `#005a6a` - Cor principal
- **Hospital Orange**: `#ff7d00` - Cor de destaque
- **Hospital Dark**: `#00313d` - Cor escura
- **Hospital Light**: `#f5f7f8` - Cor clara
 
### Tipografia
- **Fonte Principal**: Inter (Google Fonts)
- **Tamanhos**: Responsivos com TailwindCSS
 
## 📱 Funcionalidades
 
### ✅ Páginas Implementadas
- **Home** - Página inicial com hero section e especialidades
- **Especialidades** - Catálogo de especialidades médicas
- **EspecialidadeDetalhes** - Página dinâmica de detalhes da especialidade (rota com parâmetro)
- **Equipe** - Apresentação da equipe de desenvolvimento
- **FAQ** - Perguntas frequentes com accordion
- **Contato** - Formulário de contato com validação
- **Solução** - Detalhamento da solução GUIDABOT
- **Pacientes** - Listagem e gerenciamento de pacientes (CRUD)
- **PacienteForm** - Formulário de cadastro/edição de pacientes
- **NotFound (404)** - Página de erro com redirecionamento
 
### 🛣️ Rotas Implementadas
 
#### Rotas Estáticas
- `/` - Home
- `/especialidades` - Lista de especialidades
- `/equipe` - Equipe de desenvolvimento
- `/faq` - Perguntas frequentes
- `/contato` - Formulário de contato
- `/solucao` - Detalhes da solução
- `/pacientes` - Gerenciamento de pacientes
 
#### Rotas Dinâmicas (com parâmetros)
- `/especialidades/:id` - Detalhes da especialidade
- `/pacientes/novo` - Novo paciente
- `/pacientes/:id/editar` - Editar paciente
 
#### Redirecionamentos
- `/home` → `/` (redireciona para home)
- `*` → `/404` (rota não encontrada)
 
### 🔧 Hooks Utilizados
- **useState** - Gerenciamento de estado local
- **useEffect** - Efeitos colaterais e lifecycle
- **useNavigate** - Navegação programática
- **useParams** - Parâmetros de rota dinâmica
- **useForm** - Gerenciamento de formulários
- **useToast** - Hook customizado para notificações
- **useLocation** - Localização atual da rota
 
### 📋 Formulários
- **Formulário de Contato** - Validação com React Hook Form e feedback visual
- **Formulário de Paciente** - CRUD completo com validação de campos
 
### 🔌 Consumo de API REST
 
O projeto implementa consumo completo de API REST com os seguintes endpoints:
 
 
### Interfaces
- `BaseEntity` - Entidade base com ID e timestamps
- `Paciente` - Interface completa do paciente
- `Consulta` - Interface completa da consulta
- `EspecialidadeAPI` - Interface da especialidade da API
- `ApiResponse<T>` - Resposta padronizada da API
- `PaginatedResponse<T>` - Resposta paginada
- E muitas outras...
 
### Adaptações Responsivas
- Grid adaptativo (1 coluna em mobile, 2-3 em desktop)
- Navegação hambúrguer em mobile
- Tabelas com scroll horizontal em mobile
- Imagens responsivas com diferentes tamanhos
- Textos com tamanhos adaptativos
- Espaçamentos proporcionais ao tamanho da tela
 
 
## 🎯 Solução GUIDABOT
 
### Problemas Identificados
- Alta taxa de faltas e desistências (20%)
- Dificuldade de uso de tecnologias digitais
- Baixa escolaridade e analfabetismo funcional
- Falta de acompanhamento familiar
- Cadastros incompletos
 
### Nossa Solução
**GUIDABOT** - Assistente digital humanizada que:
 
1. **Cadastro Inteligente** - WhatsApp com acompanhante obrigatório
2. **Agendamento Guiado** - Validação dupla (paciente + acompanhante)
3. **Integração Externa** - Teleconsultas automatizadas
4. **Lembretes Automáticos** - Confirmação via Python
5. **Interface Acessível** - Mini site responsivo
6. **Integração IMREA** - Sistema de dados seguro
7. **Campanha Sensibilização** - Envolvimento de acompanhantes
 
### Impactos Esperados
- ✅ Redução de absenteísmo para < 10%
- ✅ Aumento do engajamento familiar
- ✅ Inclusão digital acessível
- ✅ Comunicação empática
- ✅ Cadastros 100% validados
 
## 🔗 Links Importantes
 
- **GitHub**: [https://github.com/natcsouza/Challenge-Sprint-4-FRONT-END]
- **Youtube**: [https://youtu.be/l77oVgPhylE]
 
 
## 📊 Métricas de Desenvolvimento
 
### Versionamento Git/GitHub
- **Commits por Integrante**: Mínimo 5 commits ✅
- **Total de Commits**: 15+ commits ✅
- **Branch Main**: Histórico completo preservado ✅
 
### Componentes e Páginas
- **Componentes Reutilizáveis**: 9 componentes
- **Páginas**: 10 páginas funcionais
- **Hooks Customizados**: 1 hook (useToast)
- **Serviços**: 1 serviço (api.ts)
 
### TypeScript
- **Tipos Básicos**: number, string, boolean, object ✅
- **Union Types**: 6 tipos implementados ✅
- **Intersection Types**: 2 tipos implementados ✅
- **Interfaces**: 15+ interfaces ✅
 
### API REST
- **Verbos HTTP**: GET, POST, PUT, DELETE ✅
- **Endpoints**: 15 endpoints (3 entidades x 5 operações) ✅
- **Tratamento de Erros**: Implementado ✅
- **Validação de Dados**: Implementada ✅
 
### Responsividade
- **Breakpoints**: XS, SM, MD, LG, XL, 2XL ✅
- **Layout Adaptativo**: Todos os componentes ✅
- **Navegação Mobile**: Menu hambúrguer ✅
 
### Rotas e Navegação
- Roteamento com React Router DOM v6
- Rotas estáticas e dinâmicas
- Passagem de parâmetros via URL
- Redirecionamentos programáticos
- Tratamento de rotas não encontradas (404)
 
### TypeScript Avançado
- Union Types para valores específicos
- Intersection Types para combinação de tipos
- Interfaces complexas com herança
- Tipagem genérica (Generics)
- Type guards e validação de tipos
 
### Consumo de API
- Requisições HTTP com Fetch API
- Tratamento de erros HTTP
- Validação de dados
- Feedback visual ao usuário
- Gerenciamento de estado assíncrono
 
### Responsividade
- Breakpoints do TailwindCSS
- Layout adaptativo com Grid e Flexbox
- Media queries inline
- Componentes responsivos
- Testes em diferentes dispositivos
