# react-hooks-snippets

React hooks snippets (aka [live templates](https://www.jetbrains.com/help/idea/2016.1/live-templates.html)) for JetBrains series editors

## Installation

1. Download [ReactHooks.xml](ReactHooks.xml) file and copy it to your JetBrains editor's templates folder:

    - Windows: `<your home directory>\.<product name><version number>\config\templates`
    - Linux: `~\.<product name><version number>\config\templates`
    - OS X: `~/Library/Preferences/<product name><version number>/templates`

     e.g. `~/Library/Preferences/WebStorm10/templates` on OS X for WebStorm 10

2. Restart your IDE.

3. To see all templates, go to `Preferences` -> `Live Templates` and expand the `ReactHooks` Template Group.


## Snippets

<!--DOC_START-->
### `usst`

```js
const [$VALUE$, set$CAPITALIZE_VALUE$] = useState($END$); 

```

### `usef`

```js
useEffect(() => {
   $BODY$
}, [$DEPENDENCIES$]);

```

### `usfetch`

```js
useEffect(() => {
   fetch$DATA$($DEPENDENCIES$)
}, [$DEPENDENCIES$]);

```
### `usco`

```js
const {$VALUE$} = useContext($CONTEXT$);

```

### `usm`

```js
const $VALUE$ = useMemo(() => {
$CALC_VALUE$
}, [$DEPENDENCIES$]); 

```

### `usr`

```js
const $REF$ = useRef($INIT_VALUE$);

```

