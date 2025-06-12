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

 projeto <br>
├── 📁 assets <br>
│   ├── adaptive-icon.png <br>
│   ├── favicon.png <br>
│   ├── icon.png <br>
│   ├── logo-gop.png <br>
│   └── splash-icon.png <br>
├── 📁 src <br>
│   ├── 📁 app <br>
│   │   ├── 📁 (auth) <br>
│   │   └── 📁 (tabs) <br>
│   │       ├── 📁 (adm) <br>
│   │       │   ├── AdicionarUsuarios.tsx <br>
│   │       │   ├── _layout.tsx <br>
│   │       │   └── index.tsx <br>
│   │       ├── 📁 (casos) <br>
│   │       │   ├── 📁 caso <br>
│   │       │   │   ├── [id].tsx <br>
│   │       │   │   ├── AdicionarCaso.tsx <br>
│   │       │   │   ├── AdicionarEvidencia.tsx <br>
│   │       │   │   ├── AdicionarVitima.tsx <br>
│   │       │   │   ├── _layout.tsx <br>
│   │       │   │   └── index.tsx <br>
│   │       │   ├── Dashboard.tsx <br>
│   │       │   ├── Perfil.tsx <br>
│   │       │   ├── _layout.tsx <br>
│   │       │   └── index.tsx <br>
│   ├── 📁 components <br>
│   │   ├── 📁 CardCaso <br>
│   │   │   └── index.tsx <br>
│   │   ├── 📁 CardEvidencia <br>
│   │   │   └── index.tsx <br>
│   │   ├── 📁 EditarModal <br>
│   │   │   └── index.tsx <br>
│   │   ├── 📁 ModalEvidencia <br>
│   │   │   └── index.tsx <br>
│   │   ├── 📁 OdontogramaInput <br>
│   │   │   └── OdontogramaInput.tsx <br>
│   │   ├── 📁 User <br>
│   │   │   ├── AddUserButton.tsx <br>
│   │   │   └── UserCard.tsx <br>
│   │   ├── 📁 common <br>
│   │   │   └── InputField.tsx <br>
│   │   ├── 📁 formularios-components <br>
│   │   │   ├── FormInput.tsx <br>
│   │   │   ├── ImageUploader.tsx <br>
│   │   │   ├── LocationMap.tsx <br>
│   │   │   └── PickerSelect.tsx <br>
│   ├── 📁 hook <br>
│   │   ├── useDateTimePicker.ts <br>
│   │   └── useImagePicker.ts <br>
│   ├── 📁 interfaces <br>
│   │   └── IUser.ts <br>
│   ├── 📁 lib <br>
│   │   ├── geocode.ts <br>
│   │   └── validate.ts <br>
│   ├── 📁 styles <br>
│   │   ├── AdicionarUsuarios.styles.ts <br>
│   │   ├── CadastroNovoCaso.styles.ts <br>
│   │   ├── globalStyles.ts <br>
│   │   ├── perfil.styles.ts <br>
│   │   └── vitima.styles.ts <br>
│   └── 📁 utils <br>
│       └── fileHelpers.ts <br>
├── .gitignore <br>
├── README.md <br>
├── app.json <br>
├── casos.json <br>
├── package-lock.json <br>
├── package.json <br>
└── tsconfig.json <br>

## Estrutura do Projeto

projeto <br>
├── 📁 assets/                        **# Imagens e ícones usados no app (favicon, logo, splash, etc)** <br>
│   ├── adaptive-icon.png <br>
│   ├── favicon.png <br>
│   ├── icon.png <br>
│   ├── logo-gop.png <br>
│   └── splash-icon.png <br>
│ <br>
├── 📁 src/                           **# Código-fonte principal da aplicação** <br>
│   ├── 📁 app/                       **# Arquivos relacionados às rotas e páginas** <br>
│   │   ├── 📁 (auth)/               **# Páginas de autenticação (login, cadastro)** <br>
│   │   └── 📁 (tabs)/               **# Navegação com abas principais do app** <br>
│   │       ├── 📁 (adm)/           **# Páginas exclusivas para usuários administradores** <br>
│   │       │   ├── AdicionarUsuarios.tsx     **# Tela para adicionar usuários** <br>
│   │       │   ├── _layout.tsx               **# Layout da área admin** <br>
│   │       │   └── index.tsx                 **# Página principal da aba admin** <br>
│   │       ├── 📁 (casos)/         **# Telas relacionadas à gestão de casos** <br>
│   │       │   ├── 📁 caso/                   **# Páginas de um caso específico** <br>
│   │       │   │   ├── [id].tsx                     **# Visualização de detalhes de um caso** <br>
│   │       │   │   ├── AdicionarCaso.tsx           **# Cadastro de novo caso** <br>
│   │       │   │   ├── AdicionarEvidencia.tsx      **# Adição de evidências ao caso** <br>
│   │       │   │   ├── AdicionarVitima.tsx         **# Adição de vítima ao caso** <br>
│   │       │   │   ├── _layout.tsx                 **# Layout padrão da página de caso** <br>
│   │       │   │   └── index.tsx                   **# Página principal da seção de caso** <br>
│   │       │   ├── Dashboard.tsx           **# Painel geral com estatísticas ou atalhos** <br>
│   │       │   ├── Perfil.tsx              **# Página de perfil do usuário** <br>
│   │       │   ├── _layout.tsx             **# Layout padrão da aba "casos"** <br>
│   │       │   └── index.tsx               **# Página inicial da aba "casos"** <br>
│   │ <br>
│   ├── 📁 components/                  **# Componentes reutilizáveis da interface** <br>
│   │   ├── 📁 CardCaso/              **# Card com dados de um caso** <br>
│   │   │   └── index.tsx <br>
│   │   ├── 📁 CardEvidencia/         **# Card com dados de uma evidência** <br>
│   │   │   └── index.tsx <br>
│   │   ├── 📁 EditarModal/           **# Modal para edição de dados** <br>
│   │   │   └── index.tsx <br>
│   │   ├── 📁 ModalEvidencia/        **# Modal para exibir ou adicionar evidências** <br>
│   │   │   └── index.tsx <br>
│   │   ├── 📁 OdontogramaInput/      **# Entrada gráfica para informações odontológicas** <br>
│   │   │   └── OdontogramaInput.tsx <br>
│   │   ├── 📁 User/                  **# Componentes relacionados ao usuário** <br>
│   │   │   ├── AddUserButton.tsx <br>
│   │   │   └── UserCard.tsx <br>
│   │   ├── 📁 common/                **# Componentes genéricos e utilitários (ex: input)** <br>
│   │   │   └── InputField.tsx <br>
│   │   ├── 📁 formularios-components/  **# Componentes usados em formulários diversos** <br>
│   │   │   ├── FormInput.tsx <br>
│   │   │   ├── ImageUploader.tsx <br>
│   │   │   ├── LocationMap.tsx <br>
│   │   │   └── PickerSelect.tsx <br>
│   │ <br>
│   ├── 📁 hook/                      **# Hooks personalizados para lógica reutilizável** <br>
│   │   ├── useDateTimePicker.ts <br>
│   │   └── useImagePicker.ts <br>
│   │ <br>
│   ├── 📁 interfaces/                **# Definições de tipos e interfaces TypeScript** <br>
│   │   └── IUser.ts <br>
│   │ <br>
│   ├── 📁 lib/                       **# Bibliotecas e funções auxiliares** <br>
│   │   ├── geocode.ts                       **# Função para geocodificação de endereços** <br>
│   │   └── validate.ts                      **# Funções de validação** <br>
│   │ <br>
│   ├── 📁 styles/                    **# Estilos globais e específicos das páginas** <br>
│   │   ├── AdicionarUsuarios.styles.ts <br>
│   │   ├── CadastroNovoCaso.styles.ts <br>
│   │   ├── globalStyles.ts <br>
│   │   ├── perfil.styles.ts <br>
│   │   └── vitima.styles.ts <br>
│   │ <br>
│   └── 📁 utils/                     **# Funções utilitárias diversas** <br>
│       └── fileHelpers.ts                   **# Funções auxiliares para manipulação de arquivos** <br>
│ <br>
├── .gitignore                       **# Arquivos e pastas ignorados pelo Git** <br>
├── README.md                        **# Documentação geral do projeto** <br>
├── app.json                         **# Configurações do aplicativo (Expo)** <br>
├── casos.json                       **# Arquivo de dados mock (casos)** <br>
├── package-lock.json                **# Lockfile do gerenciador de pacotes npm** <br>
├── package.json                     **# Dependências, scripts e metadados do projeto** <br>
└── tsconfig.json                    **# Configurações do compilador TypeScript** <br>



