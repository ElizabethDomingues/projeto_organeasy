# Organeasy

> **Gerenciador inteligente de tarefas e colaboração em equipe**

Um aplicativo multiplataforma desenvolvido com Flutter que facilita a organização de tarefas, gerenciamento de membros e colaboração em equipe. Perfeito para empresas, projetos de grupo e ambientes colaborativos que precisam de uma solução de gestão eficiente e intuitiva.

---

## 📋 Sumário

- [Características Principais](#-características-principais)
- [Pré-requisitos](#-pré-requisitos)
- [Instalação](#-instalação)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Como Usar](#-como-usar)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Desenvolvimento](#-desenvolvimento)


---

## ✨ Características Principais

- **Dashboard Intuitivo**: Visualize um resumo completo de tarefas, membros e salas em um só lugar
- **Gerenciamento de Tarefas**: Crie, edite, acompanhe e conclua tarefas com status customizados
- **Gerenciamento de Membros**: Adicione e gerencie membros da equipe com atribuição de tarefas
- **Organização em Salas**: Estruture seu trabalho em diferentes ambientes/projetos (salas)
- **Tema Claro/Escuro**: Alterne entre modo claro e escuro conforme sua preferência
- **Armazenamento Local**: Dados persistentes com SQLite para acesso offline
- **Multiplataforma**: Funciona em Android, iOS, Web, Windows, Linux e macOS
- **Interface Responsiva**: Design adaptável que funciona em qualquer tamanho de tela

---

## 📦 Pré-requisitos

Antes de iniciar, certifique-se de ter instalado:

- **Flutter**: Versão 3.8.0 ou superior
- **Dart**: Incluído com o Flutter
- **Git**: Para controle de versão (opcional)
- **IDE**: Visual Studio Code, Android Studio ou IntelliJ IDEA (recomendado)

### Verificar Instalação

```bash
flutter --version
dart --version
```

---

## 🚀 Instalação

### 1. Clonar o Repositório

```bash
git clone https://github.com/seu-usuario/organeasy.git
cd projeto_organeasy
```

### 2. Instalar Dependências

```bash
flutter pub get
```

### 3. Configurar o Banco de Dados

O aplicativo utiliza SQLite, que é inicializado automaticamente na primeira execução.

### 4. Executar a Aplicação

**Para dispositivo/emulador Android:**
```bash
flutter run
```

**Para iOS:**
```bash
flutter run -d ios
```

**Para Web:**
```bash
flutter run -d chrome
```

**Para Windows:**
```bash
flutter run -d windows
```

**Para macOS:**
```bash
flutter run -d macos
```

**Para Linux:**
```bash
flutter run -d linux
```

---

## 📁 Estrutura do Projeto

```
projeto_organeasy/
├── lib/
│   ├── main.dart                 # Entrada da aplicação
│   ├── model/
│   │   ├── members.dart         # Modelo de dados - Membros
│   │   ├── rooms.dart           # Modelo de dados - Salas
│   │   └── tasks.dart           # Modelo de dados - Tarefas
│   ├── screens/
│   │   ├── DashboardScreen.dart # Tela principal com resumo
│   │   ├── MembersScreen.dart   # Gerenciamento de membros
│   │   ├── RoomsScreen.dart     # Gerenciamento de salas
│   │   ├── TasksScreen.dart     # Gerenciamento de tarefas
│   │   └── settings.dart        # Configurações da aplicação
│   └── utils/
│       ├── database_helpers.dart      # Funções auxiliares de banco de dados
│       ├── members_helpers.dart       # Funções auxiliares de membros
│       ├── rooms_helpers.dart         # Funções auxiliares de salas
│       └── tasks.helpers.dart         # Funções auxiliares de tarefas
├── android/                      # Configurações específicas Android
├── ios/                          # Configurações específicas iOS
├── web/                          # Configurações específicas Web
├── windows/                      # Configurações específicas Windows
├── linux/                        # Configurações específicas Linux
├── macos/                        # Configurações específicas macOS
├── test/                         # Testes unitários e de widget
├── pubspec.yaml                  # Configuração e dependências do projeto
└── analysis_options.yaml         # Configuração de análise de código
```

---

## 💻 Como Usar

### Primeiro Acesso

1. Abra a aplicação e você verá o **Dashboard**
2. Navegue pelas abas na parte inferior para acessar diferentes funcionalidades:
   - 📊 **Dashboard**: Visão geral de tarefas e métricas
   - ✅ **Tarefas**: Crie e gerencie suas tarefas
   - 👥 **Membros**: Gerencie os membros da equipe
   - 🏠 **Salas**: Organize tarefas em diferentes ambientes/projetos
   - ⚙️ **Configurações**: Personalize a aplicação

### Criando uma Nova Tarefa

1. Acesse a aba **Tarefas**
2. Clique no botão "+" para adicionar uma nova tarefa
3. Preencha os detalhes:
   - Nome da tarefa
   - Sala/Ambiente
   - Membro responsável
   - Data de vencimento
   - Status
4. Salve a tarefa

### Gerenciando Membros

1. Acesse a aba **Membros**
2. Clique em "+" para adicionar novo membro
3. Insira o nome e selecione uma cor para identificação
4. O sistema automaticamente rastreia tarefas atribuídas e progresso

### Organizando em Salas

1. Acesse a aba **Salas**
2. Crie diferentes salas para separar projetos ou áreas
3. Atribua tarefas a salas específicas
4. Visualize o progresso por sala no Dashboard

---

## 🛠️ Tecnologias Utilizadas

### Framework
- **Flutter** (3.8.0+) - Framework multiplataforma para aplicações móveis e desktop
- **Dart** - Linguagem de programação

### Banco de Dados
- **SQLite** (`sqflite` 2.4.2+) - Banco de dados local relacional
- **sqflite_common_ffi** (2.3.5+) - Suporte FFI para SQLite em desktop

### UI/UX
- **Material Design** - Design system do Flutter
- **Google Fonts** (6.2.1+) - Tipografia moderna e variada
- **Cupertino Icons** (1.0.8+) - Ícones estilo iOS

### Utilitários
- **path_provider** (2.1.5+) - Acesso aos caminhos de diretórios do sistema

---

## 🔧 Desenvolvimento

### Executar em Modo Debug

```bash
flutter run -v
```

### Build para Release

**Android:**
```bash
flutter build apk --release
```

**iOS:**
```bash
flutter build ios --release
```

**Web:**
```bash
flutter build web --release
```

**Windows:**
```bash
flutter build windows --release
```

### Análise de Código

```bash
flutter analyze
```

### Formatação de Código

```bash
dart format .
```

### Executar Testes

```bash
flutter test
```

### Corrigir Problemas Comuns

```bash
flutter clean
flutter pub get
flutter pub upgrade
```

---

## 📱 Compatibilidade

| Plataforma | Versão Mínima | Status |
|-----------|---------------|--------|
| Android   | 5.0+          | ✅ Suportado |
| iOS       | 11.0+         | ✅ Suportado |
| Web       | Chrome 90+    | ✅ Suportado |
| Windows   | 10+           | ✅ Suportado |
| macOS     | 10.13+        | ✅ Suportado |
| Linux     | Ubuntu 18+    | ✅ Suportado |

---

## 📝 Configuração da Aplicação

A aplicação utiliza os seguintes arquivos de configuração:

- **pubspec.yaml**: Define dependências, versão e metadados do projeto
- **analysis_options.yaml**: Define regras de análise de código e linting
- **Constants**: Definidos nos helpers utilitários para customização

---

## 🤝 Contribuindo

Para contribuir com melhorias:

1. Faça um fork do repositório
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona MinhaFeature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

---

## 🐛 Reportar Problemas

Se encontrar algum bug ou ter sugestões, por favor abra uma issue no repositório com:

- Descrição clara do problema
- Passos para reproduzir
- Comportamento esperado vs. atual
- Informações do dispositivo/plataforma

---

## 📚 Recursos Úteis

- [Documentação Flutter](https://docs.flutter.dev/)
- [Flutter Cookbook](https://docs.flutter.dev/cookbook)
- [SQLite Documentation](https://www.sqlite.org/docs.html)
- [Material Design Guidelines](https://material.io/design)

---

## 📄 Licença

Este projeto está licenciado sob a Licença MIT - consulte o arquivo [LICENSE](LICENSE) para detalhes.

---

## ✉️ Suporte

Dúvidas ou sugestões? Entre em contato através de:

- **Email**: elizapdominguess@gmail.com

---

<div align="center">

**Desenvolvido com ❤️ usando Flutter**

*Última atualização: Maio de 2024*

</div>
