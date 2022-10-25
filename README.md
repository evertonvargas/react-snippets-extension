# React Fast and Productive Extension

|      Snippet | Content                                         |
| -----------: | ----------------------------------------------- |
|    `rgctx →` | React Generate Context                          |
|      `rue →` | React useEffect                                 |
|      `rus →` | React useState                                  |
|      `ref →` | React Export Function                           |
|     `recf →` | React Export Const Function                     |
|     `refn →` | React Export Function Nested                    |
|    `recfn →` | React Export Const Function Nested              |
|     `redf →` | React Export Default Function                   |
|    `redcf →` | React Export Default Const Function             |
|    `redfn →` | React Export Default Function Nested            |
|   `redcfn →` | React Export Default Const Function Nested      |
|   `ref-ts →` | React Export Function Typescript                |
|  `refn-ts →` | React Export Function Nested Typescript         |
|  `redf-ts →` | React Export Default Function Typescript        |
| `redfn-ts →` | React Export Default Function Nested Typescript |
|   `rip-ts →` | React Interface Props Typescript                |
| `rgctx-ts →` | React Generate Context Typescript               |
|      `rns →` | React Native Styles                             |
|     `rnsb →` | React Native Styles Blocks                      |
|      `jsf →` | Javascript Function                             |
|     `jscf →` | Javascript Const Function                       |
|     `jsaf →` | Javascript Async Function                       |
|     `jsac →` | Javascript Async Const Function                 |
|  `jsfetch →` | Javascript Fetch                                |
| `jsafetch →` | Javascript Async Fetch                          |
|      `cgm →` | Create Generate Media                           |
|       `sc →` | Styled Components                               |
|      `sct →` | Sytled Components Theme                         |
|  `sct:css →` | Sytled Components Theme CSS                     |

<p>
  <img src="https://raw.githubusercontent.com/evertonvargas/react-snippets-extension/vscode-extension/assets/rue.gif" width="800" title="hover text">
</p>

`start` + ((`modifier` + `action`) || `hook`) + `variant`

## Starts with

- `r` → Refers to **R**eact environment;
- `rn` → Refers to **R**eact **N**ative environment;
- `js` → **J**ava**S**cript.

## Modifiers

- `e` → export;
- `ed` → export default;
- `a` → async.

## Action

- `f` → function;
- `c` → função com constante;
- `s` → styles;
- `sb` → style block;
- `sc` → styled components.

## Variants (if available)

- `n` → nested (set component name same as folder name);
- `t` → use the TypeScript variant.

# Using with React

Everything related to React environment will use the `r` prefix.

## Specials Variant

These modifiers, at the moment, are available only within a React environment. They must be added at the end of the **_snippet query_** and must be in alphabetical order.

- `n` → It means that your current **_.tsx/.jsx_** file is nested into a folder. If used it will automatically set the created function’s name to be the same as the folder above (_father_) your file.
- `t` → This indicates that you want to use the TypeScript variant, if exists, of this snippet.

## Hooks

Can replace the modifiers and starts with **\*u** (use)\* followed by the first letter of the hook’s name:

| Snippet | Content                           |
| ------- | --------------------------------- |
| `rue`   | **_R_**eact **_u_**se**_E_**ffect |
| `rus`   | **_R_**eact **_u_**se**_S_**tate  |

<p>
  <img src="https://raw.githubusercontent.com/evertonvargas/react-snippets-extension/vscode-extension/assets/rue.gif" width="800" title="hover text">
</p>

## Exporting Components

By default, when you use the snippet to create/export a function/component it will use the current **_.tsx/.jsx_** to set its name. If you want it to use the folder’s name it is nested in, use the **_n_** variant, as you can see [here](https://github.com/evertonvargas/react-snippets-extension/tree/vscode-extension#specials-variant)

### React ( .js and Native)

When you are creating a new component you can use the following snippets to automatically generate its structure:

| Snippet | Content                                                           |
| ------- | ----------------------------------------------------------------- |
| `ref`   | **_R_**eact **_E_**xport **_F_**unction                           |
| `redf`  | **_R_**eact **_E_**xport **_D_**efault **_F_**unction             |
| `recf`  | **_R_**eact **_E_**xport **_C_**onst **_F_**unction               |
| `redcf` | **_R_**eact **_E_**xport **_D_**efault **_C_**onst **_F_**unction |

<p>
  <img src="https://raw.githubusercontent.com/evertonvargas/react-snippets-extension/vscode-extension/assets/redcf.gif" width="800" title="hover text">
</p>

If you need a typescript function with a Props Interface, you can just add a **_t_** to the end of the snippet:

| Snippet | Content                                                                  |
| ------- | ------------------------------------------------------------------------ |
| `reft`  | **_R_**eact **_E_**xport **_F_**unction (**_T_**ypeScript)               |
| `redft` | **_R_**eact **_E_**xport **_D_**efault **_F_**unction (**_T_**ypeScript) |

<p>
  <img src="https://raw.githubusercontent.com/evertonvargas/react-snippets-extension/vscode-extension/assets/redft.gif" width="800" title="hover text">
</p>

Now, if you want to go wild and use the _nested_ and _typescript_ variant **AT THE SAME TIME** (_insane…_) you should do this way:

| Snippet  | Content                                                                                   |
| -------- | ----------------------------------------------------------------------------------------- |
| `refnt`  | **_R_**eact **_E_**xport **_F_**unction (**_N_**ested and **_T_**ypeScript)               |
| `redfnt` | **_R_**eact **_E_**xport **_D_**efault **_F_**unction (**_N_**ested and **_T_**ypeScript) |

<p>
  <img src="https://raw.githubusercontent.com/evertonvargas/react-snippets-extension/vscode-extension/assets/redfnt.gif" width="800" title="hover text">
</p>

### React Native (only)

Everything exclusively related to React Native will use the `rn` prefix. When you are creating the styles of your component, you can use the following snippets to get it done quickly:

| Snippet | Content                                                |
| ------- | ------------------------------------------------------ |
| `rns`   | **_R_**eact **_N_**ative **_S_**tyles                  |
| `rnsb`  | **_R_**eact **_N_**ative **_S_**tyle **_B_**lock       |
| `rnsc`  | **_R_**eact **_N_**ative **_S_**tyled **_C_**omponents |

These only work on **_.ts/.js_** files, because are intended to be used as styles snippets

# Using with JavaScript/TypeScript

Everything related to JavaScript will use the `js` prefix. You can create functions, arrow functions and

| Snippet | Content                                                       |
| ------- | ------------------------------------------------------------- |
| `jsf`   | **_J_**ava**_S_**cript **_F_**unction                         |
| `jscf`  | **_J_**ava**_S_**cript **_C_**onst **_F_**unction             |
| `jsaf`  | **_J_**ava**_S_**cript **_A_**sync **_F_**unction             |
| `jsac`  | **_J_**ava**_S_**cript **_A_**sync **_C_**onst **_F_**unction |

<p>
  <img src="https://raw.githubusercontent.com/evertonvargas/react-snippets-extension/vscode-extension/assets/jsac.gif" width="800" title="hover text">
</p>

## JavaScript/TypeScript Utils

This section still in development and will be completed in future updates. Right now you can use soma snippets to quickly access some built-in JavaScript methods.

### Fetch

Here you can see some snippets to create a **_.fetch_**. Te _async_ one will create a

| Snippet    | Content                                        |
| ---------- | ---------------------------------------------- |
| `jsfetch`  | **_J_**ava**_S_**cript **_F_**etch             |
| `jsafetch` | **_J_**ava**_S_**cript **_A_**sync **_F_**etch |

<p>
  <img src="https://raw.githubusercontent.com/evertonvargas/react-snippets-extension/vscode-extension/assets/jsafetch.gif" width="800" title="hover text">
</p>

## Contribution

Any contribution you make will be **much appreciated**.

#### Éverton Vargas

[![Linkedin Badge](https://img.shields.io/badge/-Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/https://www.linkedin.com/in/everton-vargas/)](https://www.linkedin.com/in/everton-vargas/)
[![Github Badge](https://img.shields.io/badge/-github.com//evertonvargas-black?style=flat-square&logo=Github&logoColor=white)](https://github.com/evertonvargas)

#### Luca Rampinelli

[![Linkedin Badge](https://img.shields.io/badge/-Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/https://www.linkedin.com/in/lucarampi/)](https://www.linkedin.com/in/lucarampi/)
[![Github Badge](https://img.shields.io/badge/-github.com//lucarampi-black?style=flat-square&logo=Github&logoColor=white)](https://github.com/lucarampi)
