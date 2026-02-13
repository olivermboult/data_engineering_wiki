<div class="hero hero--navy-to-indigo">
  <h1>Wiki Contribution Guidelines</h1>
  <p>Standards, best practices, and governance for the Knowledge Hub</p>
</div>

---

## 🎯 Purpose of This Wiki

The Knowledge Hub exists to be the single source of truth for:

- **Technical documentation** – architecture patterns, design decisions, implementation guides
- **Team knowledge** – best practices, lessons learned, FAQs
- **Service offerings** – accelerators, fixed-price offerings, capabilities
- **Operational procedures** – runbooks, troubleshooting guides, standard processes

<div class="callout callout--danger">
  <p class="callout__title">❌ What this wiki is NOT for</p>
  <p class="callout__body">
    Use SharePoint/Teams for document storage, binary files (Word/PDF/Excel), and client-specific materials.
    The wiki should link to authoritative files, not duplicate them.
  </p>
</div>

---

## 🎨 Branding & Style Standards

All pages must follow the SA brand system, which is parameterised in the site stylesheet:

- **Theme variables** are defined via `data-md-color-scheme` (light/dark) and SA colour tokens
- **Reusable components** must be used instead of inline styling:
  - Hero banner: `hero`
  - Callouts: `callout` (`info`, `success`, `warning`, `danger`)
  - Page metadata footer: `page-meta`

<div class="callout callout--info">
  <p class="callout__title">ℹ️ Updating colours in one place</p>
  <p class="callout__body">To change colours across the whole site, update the SA variables in <code>docs/assets/styles/style.css</code>. Avoid hard-coded inline colours in markdown pages.</p>
</div>

---

## 📋 Page Structure Standards (Mandatory)

Every page MUST include:

1. **Title + hero banner**
2. **AI-generated notice** (only if applicable)
3. **Main content using structured headings**
4. **Page information footer (mandatory)**

---

## ✅ Content Quality Standards

All content must be:

- ✅ **Accurate** (validated, tested)
- ✅ **Current** (reflects latest practices)
- ✅ **Clear** (plain English, structured)
- ✅ **Consistent** (uses the template + components)
- ✅ **Maintainable** (ownership + review date)

<div class="callout callout--warning">
  <p class="callout__title">⚠️ AI-Generated Content Notice</p>
  <p class="callout__body">Pages containing AI-generated text must include the AI notice until reviewed and validated.</p>
</div>

---

## 🖼️ Image Management

Guidelines:

- Use descriptive file names (e.g. <code>fabric-lakehouse-architecture.png</code>)
- Optimise images where possible
- Store images under <code>docs/assets/images/</code> (recommended) and reference relatively

Example:

```markdown
![Lakehouse Architecture](../assets/images/fabric-lakehouse-architecture.png)