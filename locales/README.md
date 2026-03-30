# Adding a language

1. Copy `en.ts` to `<code>.ts`
2. Translate all values, do not change keys
3. Register the file in `index.ts`
4. Add one item to `LANGUAGE_OPTIONS`

Example:

```ts
import { de } from './de';

export const TRANSLATIONS = {
  en,
  ru,
  de
} as const;

export const LANGUAGE_OPTIONS = [
  { code: 'en', label: 'English', nativeLabel: 'English' },
  { code: 'ru', label: 'Russian', nativeLabel: 'Русский' },
  { code: 'de', label: 'German', nativeLabel: 'Deutsch' }
] as const;
```
