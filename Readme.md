# React snippets extension

[https://github.com/evertonvargas/react-snippets-extension](https://github.com/evertonvargas/react-snippets-extension)

start + modifier + (action || hook) + variant

## Starts with

- r  → Refers to React.js environment;
- rn → Refers to **R**eact **N**ative environment;
- js → JavaScript.

## Modifiers

- e → export;
- ed → export default;
- a → async.

## Action

- f → function;
- c → função com constante;
- s → styles;
- sb → style block;
- sc → styled components.

## Variants (if available)

- n → nested (set component name same as folder name);
- t → use the TypeScript variant.

# Using with React

Everything related to React environment will use the `r` prefix.

## Specials Variant

These modifiers, at the moment, are available only within a React environment. They must be added at the end of the **************snippet query************** and must be in alphabetical order.

- n → It means that your current ******.tsx******/****.jsx**** file is nested into a folder. If used it will automatically set the created function’s name to be the same as the folder above (*father*) your file.
- t → This indicates that you want to use the TypeScript variant, if exists, of this snippet.

## Hooks

Can replace the modifiers and starts with ***u** (use)* followed by the first letter of the hook’s name:

| Snippet | Content |
| --- | --- |
| rue | React useEffect |
| rus | React useState |

## Exporting Components

By default, when you use the snippet to create/export a function/component it will use the current ******.tsx******/****.jsx**** to set its name. If you want it to use the folder’s name it is nested in, use the ******n****** variant, as you can see [here](https://www.notion.so/React-snippets-extension-c51c0922967f4f12bc0fe69b2fda9aae)

### React ( .js and Native)

When you are creating a new component you can use the following snippets to automatically generate its structure: 

| Snippet | Content |
| --- | --- |
| ref | React Export Function |
| redf | React Export Default Function |
| recf | React Export Const Function |
| redcf | React Export Default Const Function |

If you need a typescript function with a Props Interface, you can just add a ***t*** to the end of the snippet:

| Snippet | Content |
| --- | --- |
| reft | React Export Function (TypeScript) |
| redft | React Export Default Function (TypeScript) |

Now, if you want to go wild and use the ******nested* and *typescript* variant **AT THE SAME TIME** (*insane…*) you should do this way:

| Snippet | Content |
| --- | --- |
| refnt | React Export Function (Nested and TypeScript) |
| redfnt | React Export Default Function (Nested and TypeScript) |

### React Native (only)

Everything exclusively related to React Native will use the `rn` prefix. When you are creating the styles of your component, you can use the following snippets to get it done quickly: 

| Snippet | Content |
| --- | --- |
| rns | React Native Styles |
| rnsb | React Native Style Block |
| rnsc | React Native Styled Components |

These only work on *******.ts/.js******* files, because are intended to be used as styles snippets

# Using with JavaScript/TypeScript

Everything related to JavaScript will use the `js` prefix. You can create functions,  arrow functions and 

| Snippet | Content |
| --- | --- |
| jsf | JavaScript Function |
| jscf | JavaScript Const Function |
| jsaf | JavaScript Async Function |
| jsac | JavaScript Async Const Function |

## JavaScript/TypeScript Utils

This section still in development and will be completed in future updates. Right now you can use soma snippets to quickly access some built-in JavaScript methods.

### Fetch

Here you can see some snippets to create a ******.fetch******. Te *async* one will create a 

| Snippet | Content |
| --- | --- |
| jsfetch | JavaScript Fetch |
| jsafetch | JavaScript Async Fetch |
