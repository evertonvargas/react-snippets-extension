# React Fast and Productive Extension

`start` + ((`modifier` + `action`) || `hook`) + `variant`

## Starts with

- `r`  → Refers to **R**eact environment;
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

These modifiers, at the moment, are available only within a React environment. They must be added at the end of the ***snippet query*** and must be in alphabetical order.

- `n` → It means that your current ***.tsx/.jsx*** file is nested into a folder. If used it will automatically set the created function’s name to be the same as the folder above (*father*) your file.
- `t` → This indicates that you want to use the TypeScript variant, if exists, of this snippet.

## Hooks

Can replace the modifiers and starts with ***u** (use)* followed by the first letter of the hook’s name:

| Snippet | Content |
| --- | --- |
| `rue` | ***R***eact ***u***se***E***ffect |
| `rus` | ***R***eact ***u***se***S***tate |

## Exporting Components

By default, when you use the snippet to create/export a function/component it will use the current ***.tsx/.jsx*** to set its name. If you want it to use the folder’s name it is nested in, use the ***n*** variant, as you can see [here](https://github.com/evertonvargas/react-snippets-extension/tree/vscode-extension#specials-variant)

### React ( .js and Native)

When you are creating a new component you can use the following snippets to automatically generate its structure: 

| Snippet | Content |
| --- | --- |
| `ref` | ***R***eact ***E***xport ***F***unction |
| `redf` | ***R***eact ***E***xport ***D***efault ***F***unction |
| `recf` | ***R***eact ***E***xport ***C***onst ***F***unction |
| `redcf` | ***R***eact ***E***xport ***D***efault ***C***onst ***F***unction |

If you need a typescript function with a Props Interface, you can just add a ***t*** to the end of the snippet:

| Snippet | Content |
| --- | --- |
| `reft` | ***R***eact ***E***xport ***F***unction (***T***ypeScript) |
| `redft` | ***R***eact ***E***xport ***D***efault ***F***unction (***T***ypeScript) |

Now, if you want to go wild and use the *nested* and *typescript* variant **AT THE SAME TIME** (*insane…*) you should do this way:

| Snippet | Content |
| --- | --- |
| `refnt` | ***R***eact ***E***xport ***F***unction (***N***ested and ***T***ypeScript) |
| `redfnt` | ***R***eact ***E***xport ***D***efault ***F***unction (***N***ested and ***T***ypeScript) |

### React Native (only)

Everything exclusively related to React Native will use the `rn` prefix. When you are creating the styles of your component, you can use the following snippets to get it done quickly: 

| Snippet | Content |
| --- | --- |
|`rns`| ***R***eact ***N***ative ***S***tyles |
|`rnsb` | ***R***eact ***N***ative ***S***tyle ***B***lock |
|`rnsc` | ***R***eact ***N***ative ***S***tyled ***C***omponents |

These only work on ***.ts/.js*** files, because are intended to be used as styles snippets

# Using with JavaScript/TypeScript

Everything related to JavaScript will use the `js` prefix. You can create functions,  arrow functions and 

| Snippet | Content |
| --- | --- |
| `jsf` | ***J***ava***S***cript ***F***unction |
| `jscf` | ***J***ava***S***cript ***C***onst ***F***unction |
| `jsaf` | ***J***ava***S***cript ***A***sync ***F***unction |
| `jsac` | ***J***ava***S***cript ***A***sync ***C***onst ***F***unction |

## JavaScript/TypeScript Utils

This section still in development and will be completed in future updates. Right now you can use soma snippets to quickly access some built-in JavaScript methods.

### Fetch

Here you can see some snippets to create a ***.fetch***. Te *async* one will create a 

| Snippet | Content |
| --- | --- |
| `jsfetch` | ***J***ava***S***cript ***F***etch |
| `jsafetch` | ***J***ava***S***cript ***A***sync ***F***etch |

## Contribution
Any contribution you make will be **much appreciated**.

#### Éverton Vargas

[![Linkedin Badge](https://img.shields.io/badge/-Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/https://www.linkedin.com/in/everton-vargas/)](https://www.linkedin.com/in/everton-vargas/) 
[![Github Badge](https://img.shields.io/badge/-github.com//evertonvargas-black?style=flat-square&logo=Github&logoColor=white)](https://github.com/evertonvargas)

#### Luca Rampinelli
[![Linkedin Badge](https://img.shields.io/badge/-Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/https://www.linkedin.com/in/lucarampi/)](https://www.linkedin.com/in/lucarampi/) 
[![Github Badge](https://img.shields.io/badge/-github.com//lucarampi-black?style=flat-square&logo=Github&logoColor=white)](https://github.com/lucarampi)
