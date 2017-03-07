# Input Component API

The intent of this guide is to standardise input component API .

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", 
and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](http://www.ietf.org/rfc/rfc2119.txt).

## 1. Specification

- Component name MUST start with `input-`.
- Component MUST support `v-model` directive.
- Component SHOULD NOT use [global](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes), [input](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input), [select](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/select) and [textarea](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/textarea) attribute names as prop names.
- Component MAY use [global](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes), [input](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input), [select](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/select) and [textarea](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/textarea) attribute names as prop names if prop provides the same functionality.
- Component SHOULD NOT use [WebAPI event](https://developer.mozilla.org/en-US/docs/Web/API/Event) names.
- Component SHOULD NOT leak styles.

## 2. Examples

``` js
...
  props: {
    value: {
      type: ...,
      required: true
    }
...

```
