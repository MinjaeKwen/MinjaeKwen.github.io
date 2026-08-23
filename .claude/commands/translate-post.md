# translate-post

**Scope**: minjaekwen.com personal website (`MinjaeKwen.github.io`)
**Purpose**: Translate a blog post between Korean and English and create the corresponding `.md` file in `blog/_posts/`.

---

## Steps

1. **Identify the source file** — read its front matter and note: `lang`, `ref`, `hidden`, `date`, `thumbnail`, `title`

2. **Create the translated file** in `blog/_posts/` using the same date and an appropriate slug

3. **Front matter rules**:
   - `lang`: flip (`ko` → `en` or `en` → `ko`)
   - `ref`: keep identical to source (links the two files as a translation pair)
   - `hidden`: flip from source — only one version should appear in the blog list at a time
   - `date`, `thumbnail`: keep identical to source
   - `title`: translate, and append `[KOR]` or `[ENG]` suffix as appropriate

4. **First line of body** — add translation notice in bold:
   - English translation: `**\* This English translation is provided by Claude.**`
   - Korean translation: `**\* Claude가 번역한 한국어 버전입니다.**`

5. **Translate the full body** — before translating each sentence, first understand the surrounding context within the paragraph as a whole, then choose English expressions that fit naturally within that context rather than translating word-for-word. Preserve all image paths, URLs, and markdown formatting exactly.

6. Present the created file and ask for confirmation before pushing (follow standard Workflow in CLAUDE.md)
