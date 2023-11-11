# Coding Style

### .editorconfig

For IDE related style, related to indent, space etc. Eg.:

```editorconfig
# EditorConfig is awesome: https://EditorConfig.org

# top-most EditorConfig file
root = true

# Unix-style newlines with a newline ending every file
[*]
charset = utf-8
end_of_line = lf
indent_size = 2
indent_style = space
insert_final_newline = true
trim_trailing_whitespace = true
quote_type = single
# 4 space indentation
[*.py]
indent_style = space
indent_size = 4

# Indentation override for all JS under lib directory
[lib/**.js]
indent_style = space
indent_size = 2
```

### .eslintrc.\*

For local configuration of ES Lint.
eg.
`eslintrc.json`

```json
{
  "env": {
    "browser": true,
    "commonjs": true,
    "es2021": true
  },
  "extends": ["eslint:recommended"],
  "parserOptions": {
    "ecmaVersion": "latest"
  },
  "rules": {
    "semi": ["error", "always"],
    "quotes": ["error", "single"]
  }
}
```

### .prettierrc

For local configuration of prettier, to format based on those rules.
eg.

```json
{
  "singleQuote": true,
  "trailingComma": "all"
}
```
