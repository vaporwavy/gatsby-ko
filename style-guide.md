# Style Guide

Use this file for language-specific style rules to follow for translation.

## Rules

### Text in Code Blocks

Leave text in code blocks untranslated except for comments. You may optionally translate text in strings, but be careful not to translate strings that refer to code!

Example:

```js
// Example
import React from "react"
export default () => (
  <div style={{ color: `purple`, fontSize: `72px` }}>Hello Gatsby!</div>
)
```

✅ DO:

```js
// Ejemplo
import React from "react"
export default () => (
  <div style={{ color: `purple`, fontSize: `72px` }}>Hello Gatsby!</div>
)
```

✅ ALSO OKAY:

```js
// Ejemplo
import React from "react"
export default () => (
  <div style={{ color: `purple`, fontSize: `72px` }}>¡Hola Gatsby!</div>
)
```

❌ DON'T:

```js
// Ejemplo
import React from "react"
export default () => (
  // 'purple' is a CSS keyword
  <div style={{ color: `morado`, fontSize: `72px` }}>¡Hola Gatsby!</div>
)
```

❌ DEFINITELY DON'T:

```js
importar Reaccionar desde "reaccionar"
exportar defecto () => (
   <div estilo = {{color: `morado`, fontSize:` 72px`}}> ¡Hola Gatsby! </div>
)
```

### External Links

If an external link is to an article in a reference like [MDN] or [Wikipedia], and a version of that article exists in your language that is of decent quality, consider linking to that version instead.

[mdn]: https://developer.mozilla.org/en-US/
[wikipedia]: https://en.wikipedia.org/wiki/Main_Page

Example:

```md
React elements are [immutable](https://en.wikipedia.org/wiki/Immutable_object).
```

✅ OK:

```md
Los elementos de React son [inmutables](https://es.wikipedia.org/wiki/Objeto_inmutable).
```

For links that have no equivalent (Stack Overflow, YouTube videos, etc.), just use the English link.

## Glossary

Use this section to list how common technical terminology should be translated.

| Term                | Translation  |
| ------------------- | ------------ |
| Gatsby              | Gatsby       |
| Plugin              | 플러그인       |
| Theme               | 테마          |
| Query               | 쿼리          |
| boilerplate         | 보일러 플레이트  |
| (React)Components   | 컴포넌트       |
| CSS Module          | CSS Module    |
| Starter             | 문맥에 따라 스타터 또는 starter |
| Library             | 라이브러리       |
| guide               | 가이드          |
| tutorial            | 튜토리얼        |
| Data sourcing       | 데이터 소싱      |
| source              | 문맥에 따라 source 또는 소스 |
