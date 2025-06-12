# readmefront

<h2>Introdução</h2>
O GOP - Gestão odontolegal pericial - serve para facilitar o dia a dia das autoridades, através de um design limpo e intuitivo feito especialmente para que todos os públicos possam usá-lo. Além disso, irá ajudar na organização dos casos, a fim de agilizá-los melhorando a visualização do mesmo. Além disso, será possível fazer tudo isso através do celular, tirando fotos e cadastrando evidências de forma ágil.

<h2>Tecnologias</h2>
<h2>Tecnologias</h2>
<ul>
  <li><strong>React Native</strong></li>
  <li><strong>React Native Paper</strong></li>
  <li><strong>Expo</strong></li>
  <li><strong>Gemini</strong></li>
</ul>


<h2>Funcionalidades</h2>
<ul>
<li>Visualizar todos os casos com cores diferentes, conforme o status de cada caso.</li>
  <li>Visualizar detalhes de um caso específico.</li>
  <li>Adicionar um novo caso preenchendo um formulário completo.</li>
  <li>Listar todas as evidências de um caso.</li>
  <li>Gerar relatório de um caso encerrado.</li>
  <li>Fazer download em PDF das evidências de um caso encerrado.</li>
  <li>Visualizar informações detalhadas de uma evidência.</li>
  <li>Fazer download individual de evidências.</li>
  <li>Adicionar novas evidências a um caso, realizando upload de arquivos.</li>
  </ul>
<br>

 projeto <br>
## Estrutura do Projeto

```bash
projeto/
├── 📁 assets/                          # Recursos visuais da aplicação
│   ├── adaptive-icon.png
│   ├── favicon.png
│   ├── icon.png
│   ├── logo-gop.png
│   └── splash-icon.png
│
├── 📁 src/                             # Código-fonte da aplicação
│   ├── 📁 app/                         # Rotas e páginas principais
│   │   ├── 📁 (auth)/                 # Telas de autenticação (login, etc)
│   │   └── 📁 (tabs)/                 # Telas com navegação por abas
│   │       ├── 📁 (adm)/             # Telas administrativas
│   │       │   ├── AdicionarUsuarios.tsx       # Tela de adicionar usuário
│   │       │   ├── _layout.tsx                 # Layout padrão da seção
│   │       │   └── index.tsx                   # Página inicial da seção admin
│   │       ├── 📁 (casos)/           # Gestão de casos
│   │       │   ├── 📁 caso/                   # Operações sobre um caso específico
│   │       │   │   ├── [id].tsx                     # Visualização detalhada de um caso
│   │       │   │   ├── AdicionarCaso.tsx           # Cadastro de novo caso
│   │       │   │   ├── AdicionarEvidencia.tsx      # Adição de evidência
│   │       │   │   ├── AdicionarVitima.tsx         # Adição de vítima
│   │       │   │   ├── _layout.tsx                 # Layout padrão da seção
│   │       │   │   └── index.tsx                   # Página inicial de casos
│   │       │   ├── Dashboard.tsx           # Painel de controle
│   │       │   ├── Perfil.tsx              # Tela de perfil
│   │       │   ├── _layout.tsx             # Layout principal da aba "casos"
│   │       │   └── index.tsx               # Tela principal da aba "casos"
│
│   ├── 📁 components/                    # Componentes reutilizáveis
│   │   ├── 📁 CardCaso/                # Card de exibição de casos
│   │   │   └── index.tsx
│   │   ├── 📁 CardEvidencia/           # Card para evidências
│   │   │   └── index.tsx
│   │   ├── 📁 EditarModal/             # Modal de edição
│   │   │   └── index.tsx
│   │   ├── 📁 ModalEvidencia/          # Modal para evidências
│   │   │   └── index.tsx
│   │   ├── 📁 OdontogramaInput/        # Componente de entrada odontológica
│   │   │   └── OdontogramaInput.tsx
│   │   ├── 📁 User/                    # Componentes relacionados a usuários
│   │   │   ├── AddUserButton.tsx
│   │   │   └── UserCard.tsx
│   │   ├── 📁 common/                  # Componentes genéricos
│   │   │   └── InputField.tsx
│   │   ├── 📁 formularios-components/  # Componentes específicos de formulários
│   │   │   ├── FormInput.tsx
│   │   │   ├── ImageUploader.tsx
│   │   │   ├── LocationMap.tsx
│   │   │   └── PickerSelect.tsx
│
│   ├── 📁 hook/                        # Hooks personalizados
│   │   ├── useDateTimePicker.ts
│   │   └── useImagePicker.ts
│
│   ├── 📁 interfaces/                  # Interfaces TypeScript
│   │   └── IUser.ts
│
│   ├── 📁 lib/                         # Funções auxiliares
│   │   ├── geocode.ts
│   │   └── validate.ts
│
│   ├── 📁 styles/                      # Estilos globais e específicos
│   │   ├── AdicionarUsuarios.styles.ts
│   │   ├── CadastroNovoCaso.styles.ts
│   │   ├── globalStyles.ts
│   │   ├── perfil.styles.ts
│   │   └── vitima.styles.ts
│
│   └── 📁 utils/                       # Funções utilitárias
│       └── fileHelpers.ts
│
├── .gitignore                         # Arquivos/pastas ignorados pelo Git
├── README.md                          # Documentação do projeto
├── app.json                           # Configuração do app (Expo)
├── casos.json                         # Dados mock de casos
├── package-lock.json                  # Lockfile do npm
├── package.json                       # Dependências e scripts do projeto
└── tsconfig.json                      # Configurações do TypeScript
```

