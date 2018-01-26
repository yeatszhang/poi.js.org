# library

### format

Type: `string`<br>
Default: `undefined`<br>
Possible values: `cjs` `umd`

Set the format of output bundle.

### library

Type: `boolean` `string`

Build your app as a library.

- `boolean`: Build in CommonJS format, output [filename](#filename) will default to current folder name in kebab case.
- `string`: Build in UMD format, and we set [moduleName](#modulename) to its value. Output filename will default to the moduleName in kebab case.

<p class="tip">
  Note that [html](#html), [sourceMap](#sourcemap) are also disabled when building as library.
</p>

### moduleName

Type: `string`

Only required when `format` is set to `umd`, basically it's the same as [output.library](https://webpack.js.org/configuration/output/#output-library) in raw webpack config.