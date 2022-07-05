# Angular VSCode Extension Pack

![angular-badge]

This extension pack packages some of the most popular (and some I find very useful) VS Code Angular extensions.

## Extensions Included

### Angular + Angular Material + NgRX + RxJS Code Snippets

* [Angular Snippets](https://marketplace.visualstudio.com/items?itemName=johnpapa.Angular2) - Angular with TypeScript snippets.

* [Angular Material 2, Flex layout 1, Covalent 1 & Material icon snippets](https://marketplace.visualstudio.com/items?itemName=1tontech.angular-material) - Angular Material and Angular FlexBox component snippets.

* [Angular File Changer (Supporting Touch Bar and NgRx)](https://marketplace.visualstudio.com/items?itemName=john-crowson.angular-file-changer) - Navigate between Angular component's relative files or NgRx files using your Mac Touch Bar or keyboard.

* [angular2-switcher](https://marketplace.visualstudio.com/items?itemName=infinity1207.angular2-switcher) - Easily navigate to typescript(.ts)|template(.html)|style(.scss/.sass/.less/.css) in angular projects.
  - `alt+o`(Windows) or `shift+alt+o`(macOS)
  - by default VSCode opens file not opened from file explorer in 'preview' mode. When using this extension, I also recommend the following setting: `workbench.editor.enablePreview": false`

### Testing

* [SimonTest](https://marketplace.visualstudio.com/items?itemName=SimonTest.simontest) - Analyzes your Angular code and generates unit tests for you (can overwrite spec files generated automatically with Angular CLI).

* [Karma Problem Matcher](https://marketplace.visualstudio.com/items?itemName=rctay.karma-problem-matcher) - Capture errors from Karma tests running in Visual Studio Code, so test failures will show up in 'Problems' pane (Ctrl+Shift+M on Windows/Linux, ⇧⌘M on Mac) and the failing test can also be made known to VS Code, eg. highlighted with squiggly lines, jumping to it with F8.

### Template Productivity

* [Angular Language Service](https://marketplace.visualstudio.com/items?itemName=Angular.ng-template) - provides a rich editing experience for Angular templates, very useful when working on Angular HTML template.

* [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag) - Auto rename paired HTML/XML tag.

* [Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag) - Automatically add HTML/XML close tag, same as Visual Studio IDE or Sublime Text.

* [Arrr](https://marketplace.visualstudio.com/items?itemName=obenjiro.arrr) - a tool to refactor components from HTML templates

### Productivity

* [Auto Import](https://marketplace.visualstudio.com/items?itemName=steoates.autoimport) - Automatically finds, parses and provides code actions and code completion for all available imports (altough VSCode has auto import funcionatlity, this plugin is a great complement).

* [Paste JSON as Code](https://marketplace.visualstudio.com/items?itemName=quicktype.quicktype) - Convert a JSON from clipboard to TypeScript interfaces.

* [Prettier - JavaScript formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) - format your Javascript / Typescript / CSS - specially for Angular, I recommend adding the following config in you users setting for VsCode. Recommended settings:
  - `"prettier.singleQuote": true` (this helps when using auto import extension or the VSCode auto import functionality).
  - `"prettier.tabWidth": 2` (angular lint uses 2 spaces as default indentation). With this setting, you can continue using tabs if it is your preference
  - `"prettier.useTabs": false` (same as above)
 
 * [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense) - VSCode has a very good auto import capability, but sometime you still need to import some files manually, and this extension helps a lot in these cases.
 
 * [Move TS](https://marketplace.visualstudio.com/items?itemName=stringham.move-ts) - this is a great extension to help you refactor and re-organize some files and components in the project. It automatically fixes the imports on the file (or component folder) that is being moved and also files that are importing the component you are moving. To use it: right-click on a file or folder in the Project Explorer pane and select 'Move TypeScript'.

 * [Angular Schematics](https://marketplace.visualstudio.com/items?itemName=cyrilletuzi.angular-schematics) - this extension allows you to launch Angular schematics (CLI commands) from files Explorer (right-click) or Command Palette.

 * [Angular-cli](https://marketplace.visualstudio.com/items?itemName=segerdekort.angular-cli) - This extension eases the use of the Angular cli in Visual Studio Code.

### Code Analysis

* [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

* [TypeScript Hero](https://marketplace.visualstudio.com/items?itemName=rbbit.typescript-hero) - Favorite feature for Angular projects: sorts and organizes your imports according to convention and removes imports that are unused (`Ctrl+Alt+o` on Win/Linux or `Ctrl+Opt+o` on MacOS).

### Git

* [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) - Supercharge Git within VS Code — Visualize code authorship at a glance via Git blame annotations and CodeLens, seamlessly navigate and explore Git repositories, gain valuable insights via rich visualizations and powerful comparison commands, and so much more

* [Git History](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory) - View git log, file history, compare branches or commits

### Workbench

* [EditorConfig for VS Code](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig) - EditorConfig Support for Visual Studio Code (must have plugin for VSCode)

* [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme) - Material Design Icons for Visual Studio Code

### Other

* [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) - Launch a development local Server with live reload feature for static & dynamic pages



## Development

- Clone the repo

```bash
$ git clone https://github.com/carloscostales/vscode-angular-pack.git
```

- Install vsce

```bash
$ npm install -g vsce
```

- Build the extension file

```bash
$ vsce package
```

- Install the extension from a package file (.vsix)

1. Launch Visual Studio Code
2. Choose **Extensions** from menu
3. Click **More** > **Install from VSIX...**
4. Select the file `vscode-extension-pack-x.x.x.vsix`
5. Click **Reload Now** to reload the Code

## Publishing

- Create a publisher

```bash
$ vsce create-publisher <publisher-name>
```

- Login

```bash
$ vsce login <publisher-name>
```

- Publish

```bash
$ vsce publish
```

## Author

[Carlos Costales](https://github.com/carloscostales)

[angular-badge]: https://upload.wikimedia.org/wikipedia/commons/c/ca/AngularJS_logo.svg