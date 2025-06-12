# readmefront

<h2>Introdução</h2>
O GOP - Gestão odontolegal pericial - serve para facilitar o dia a dia das autoridades, através de um design limpo e intuitivo feito especialmente para que todos os públicos possam usá-lo. Além disso, irá ajudar na organização dos casos, a fim de agilizá-los melhorando a visualização do mesmo. Além disso, será possível fazer tudo isso através do celular, tirando fotos e cadastrando evidências de forma ágil.

<h2>Tecnologias</h2>

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
