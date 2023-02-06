# react-hooks-snippets

React hooks snippets (aka [live templates](https://www.jetbrains.com/help/idea/2016.1/live-templates.html)) for JetBrains series editors.  
Also here is a repository with [redux-boilerplate-snippets](https://github.com/TanyaIgnatenko/redux-boilerplate-snippets).

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
const [$VALUE$, set$CAPITALIZED_VALUE$] = useState$END$($INIT_VALUE$); 

```

### `usred`

```js
const [$STATE$, dispatch] = useReducer$END$($REDUCER$, $INIT_VALUE$); 

```

### `usef`

```js
useEffect$END$(() => {
   $BODY$
}, [$DEPENDENCIES$]);

```
### `usco`

```js
const {$VALUE$} = useContext$END$($CONTEXT$);

```

### `usm`

```js
const $VALUE$ = useMemo$END$(() => {
$CALC_VALUE$
}, [$DEPENDENCIES$]); 

```

### `usref`

```js
const $REF$ = useRef$END$($INIT_VALUE$);

```

### `uscall`

```js
const $CALLBACK$ = useCallback$END$(
  () => {
    $DO_SOMETHING$
  },
  [$DEPENDENCIES$],
);

```

### `usloc`

```js
const location = useLocation$END$(); 

```
### `ushist`

```js
const history = useHistory$END$();

```

### `ussel`

```js
const $DATA$ = useSelector$END$(select$METHOD_NAME$, $EQUALITY_FN$);

```

### `ussel-param`

```js
const $DATA$ = useSelector$END$(state =>
        select$METHOD_NAME$(state,  $PARAMS$),
        $EQUALITY_FN$
);

```
