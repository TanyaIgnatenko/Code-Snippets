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
const [$VALUE$, set$CAPITALIZED_VALUE$] = useState($INIT_VALUE$); 

```

### `usred`

```js
const [state, dispatch] = useReducer($REDUCER$, $INIT_VALUE$); 

```

### `usmultistate`

```js
const [state, setState] = useReducer($REDUCER$, $INIT_VALUE$); 

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

### `usref`

```js
const $name$Ref = useRef($INIT_VALUE$);

```

### `uscall`

```js
const $CALLBACK$ = useCallback(
  () => {
    $DO_SOMETHING$
  },
  [$DEPENDENCIES$],
);

```
## Extra
### `usinpust`

```js
const [$VALUE$, handle$CAPITALIZE_VALUE$Change] = useInputState($INIT_VALUE$); 

```
### `uschest`

```js
const [$VALUE$, handle$CAPITALIZE_VALUE$Change] = useCheckboxState($INIT_VALUE$); 

```

### `usinpur`

```js
const [inputsState, handleChange] = useInputsReducer($INIT_VALUE$); 

```
