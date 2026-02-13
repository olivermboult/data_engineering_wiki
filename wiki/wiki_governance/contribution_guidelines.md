# Wiki Contribution Guidelines

<div style="text-align: center; padding: 40px 20px; background: linear-gradient(135deg, #1B3A52 0%, #2E5984 100%); border-radius: 8px; margin: 20px 0;">
  <h1 style="font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; font-size: 48px; font-weight: 700; color: #ffffff; margin: 0 0 20px 0; text-shadow: 2px 2px 4px rgba(0,0,0,0.2);">
    Wiki Contribution Guidelines
  </h1>
  <p style="font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; font-size: 20px; color: #F5F7FA; margin: 0; font-weight: 400;">
    Standards, best practices, and governance for the Simpson Associates Knowledge Hub
  </p>
</div>

---

## 🎯 Purpose of This Wiki

The **Simpson Associates Knowledge Hub** serves as the single source of truth for:

- **Technical documentation** - Architecture patterns, design decisions, implementation guides
- **Team knowledge** - Best practices, lessons learned, FAQs
- **Service offerings** - Accelerators, fixed-price offerings, capabilities
- **Operational procedures** - Runbooks, troubleshooting guides, standard processes

### ❌ What This Wiki is NOT For

- **Document storage** - Store documents in SharePoint/Teams, link to them from the wiki
- **Project-specific files** - Keep project files in their respective repositories or SharePoint sites
- **Binary files** - PDFs, Word docs, Excel files belong in SharePoint/Teams
- **Temporary notes** - Use OneNote or Teams for working notes
- **Client-specific data** - Store in client-specific SharePoint sites with appropriate access controls

---

## 🎨 Simpson Associates Branding Standards

### Brand Colors

All wiki content MUST use Simpson Associates brand colors, not generic Azure blue:

**Primary Colors:**
- **Simpson Navy:** `#1B3A52` - Primary headers, table headers, key elements
- **Simpson Indigo:** `#2E5984` - Secondary headers, accents
- **Simpson Slate:** `#4A5F75` - Tertiary elements, borders

**Accent Colors:**
- **Simpson Teal:** `#0A7A8A` - Highlights, links, call-outs
- **Simpson Orange:** `#E67E22` - Warning banners, important notices
- **Simpson Green:** `#27AE60` - Success indicators, positive states
- **Simpson Red:** `#C0392B` - Deprecation notices, critical warnings

**Neutral Colors:**
- **White:** `#FFFFFF` - Backgrounds
- **Light Gray:** `#F5F7FA` - Alternate row backgrounds
- **Medium Gray:** `#D0D4D9` - Borders
- **Dark Gray:** `#1A1A1A` - Body text

### Typography

**Preferred Font Family:** Silka (as per Brand Guidelines 2025)
- **Headings:** Silka Bold
- **Body Text:** Silka Regular
- **Code/Monospace:** Consolas, 'Courier New', monospace

**Font Specifications:**
```css
/* Headings */
font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;
font-weight: 700;

/* Body Text */
font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;
font-weight: 400;
```

**Installing Silka Fonts (Recommended):**

To see wiki content with the proper Simpson Associates branding fonts:

1. Download the Silka font family from the Brand Guidelines package
2. Install the fonts on your system:
   - **Windows:** Right-click font files → Install for all users
   - **macOS:** Double-click font files → Install Font
   - **Linux:** Copy to `~/.local/share/fonts/` and run `fc-cache -f`
3. Restart your browser to apply the fonts

When Silka is installed, all styled elements in the wiki will render with the correct brand typography. If not installed, the wiki will fall back to system fonts (Segoe UI, Arial, etc.).

### Visual Identity Guidelines

1. **Use brand colors consistently** - Replace any instances of Azure blue (#1B3A52) with Simpson Navy (#1B3A52)
2. **Table headers** - Use Simpson Navy background with white text
3. **Callout boxes** - Use Simpson Teal for informational, Simpson Orange for warnings
4. **Links** - Use Simpson Teal for consistency
5. **Logo usage** - When adding Simpson Associates logo, use official files from brand guidelines
### Hero Banner (RECOMMENDED)

**All wiki pages SHOULD include a hero banner** for consistent visual branding and improved user experience.

**Standard Hero Banner Template:**
```html
<div style="text-align: center; padding: 40px 20px; background: linear-gradient(135deg, #1B3A52 0%, #2E5984 100%); border-radius: 8px; margin: 20px 0;">
  <h1 style="font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; font-size: 48px; font-weight: 700; color: #ffffff; margin: 0 0 20px 0; text-shadow: 2px 2px 4px rgba(0,0,0,0.2);">
    Page Title
  </h1>
  <p style="font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; font-size: 20px; color: #F5F7FA; margin: 0; font-weight: 400;">
    Brief description or tagline
  </p>
</div>
```

**Gradient Color Schemes by Section:**

- **Azure Landing Zones:** Navy to Indigo `linear-gradient(135deg, #1B3A52 0%, #2E5984 100%)`
- **Data & Analytics:** Teal to Indigo `linear-gradient(135deg, #0A7A8A 0%, #2E5984 100%)`
- **Team Resources:** Indigo to Navy `linear-gradient(135deg, #2E5984 0%, #1B3A52 100%)`
- **Knowledge Base:** Slate to Indigo `linear-gradient(135deg, #4A5F75 0%, #2E5984 100%)`
- **Service Offerings:** Navy to Teal `linear-gradient(135deg, #1B3A52 0%, #0A7A8A 100%)`

### Callout & Notice Box Styling

**Informational Callout (Simpson Teal):**
```html
<div style="border-left: 4px solid #0A7A8A; padding: 15px; margin: 20px 0; background-color: #F5F7FA;">
  <p style="font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; color: #0A7A8A; font-weight: bold; margin-bottom: 5px;">ℹ️ Information</p>
  <p style="font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; color: #4A5F75; margin: 0;">Your informational content here</p>
</div>
```

**Warning Notice (Simpson Orange):**
```markdown
> ⚠️ **Warning Notice**  
> Use standard markdown blockquote for warning notices
```

**Success/Tip (Simpson Green):**
```html
<div style="border-left: 4px solid #27AE60; padding: 15px; margin: 20px 0; background-color: #F5F7FA;">
  <p style="font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; color: #27AE60; font-weight: bold; margin-bottom: 5px;">✅ Success</p>
  <p style="font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; color: #4A5F75; margin: 0;">Your success message here</p>
</div>
```

**Deprecation Notice (Simpson Red):**
```html
<div style="border-left: 4px solid #C0392B; padding: 15px; margin: 20px 0; background-color: #FFEBEE;">
  <p style="font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; color: #C0392B; font-weight: bold; margin-bottom: 5px;">🚫 DEPRECATED</p>
  <p style="font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; color: #1a1a1a; margin: 0;">This content is no longer maintained</p>
</div>
```
### Table Styling Standards

**Header Row:**
```html
<tr style="background-color: #1B3A52;">
  <th style="padding: 12px; border: 2px solid #1B3A52; text-align: left; color: #ffffff; font-weight: bold;">Header</th>
</tr>
```

**Data Rows:**
```html
<tr>
  <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Content</td>
  <td style="padding: 12px; background-color: #F5F7FA; border: 2px solid #D0D4D9; color: #1a1a1a;">Content</td>
</tr>
```

---

## 📋 Wiki Structure Standards

### Page Organization

Every wiki page MUST follow this structure:

```markdown
# Page Title – Subtitle (if applicable)

<div style="text-align: center; padding: 40px 20px; background: linear-gradient(135deg, #1B3A52 0%, #2E5984 100%); border-radius: 8px; margin: 20px 0;">
  <h1 style="font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; font-size: 48px; font-weight: 700; color: #ffffff; margin: 0 0 20px 0; text-shadow: 2px 2px 4px rgba(0,0,0,0.2);">
    Page Title
  </h1>
  <p style="font-family: 'Silka', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; font-size: 20px; color: #F5F7FA; margin: 0; font-weight: 400;">
    Brief description or tagline
  </p>
</div>

---

> ⚠️ **AI-Generated Content Notice**  
> This document contains AI-generated content and is currently under review. Details may require validation.

---

[MAIN CONTENT HERE]

---

## 📄 Page Information

**Page created:** [Month Year]  
**Last modified:** [DD/MM/YYYY]  
**Last reviewed by:** [Name]  
**Next review due:** [DD/MM/YYYY]  
**Maintained by:** [Team Name or Individual]
```

### Folder Structure

```
SA-Knowledge-Hub.wiki/
├── Cloud-Platform-Team/
│   ├── Azure-Landing-Zones/
│   │   └── [Service]/
│   │       ├── Overview.md
│   │       ├── Architecture.md
│   │       ├── Delivery-Approach.md
│   │       └── Implementation-Guide.md
│   ├── Data-&-Analytics/
│   ├── Service-Offerings/
│   └── Team-Resources/
└── .attachments/
    └── [referenced-images-only]
```

---

## ✅ Content Quality Standards

### 1. AI-Generated Content Notice

**ALL pages containing AI-generated content MUST include the warning banner:**

```markdown
> ⚠️ **AI-Generated Content Notice**  
> This document contains AI-generated content and is currently under review. Details may require validation.
```

**Remove this notice only after:**
- Content has been thoroughly reviewed by a subject matter expert
- Technical accuracy has been validated
- All code examples have been tested

---

### 2. Page Footer (MANDATORY)

Every page MUST include a footer with:

<div style="width: 100%; max-width: 1000px; margin: 20px auto;">
  <table style="width: 100%; border-collapse: collapse;">
    <tr style="background-color: #1B3A52;">
      <th style="padding: 12px; border: 2px solid #1B3A52; text-align: left; color: #ffffff; font-weight: bold;">Field</th>
      <th style="padding: 12px; border: 2px solid #1B3A52; text-align: left; color: #ffffff; font-weight: bold;">Description</th>
      <th style="padding: 12px; border: 2px solid #1B3A52; text-align: left; color: #ffffff; font-weight: bold;">Example</th>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Page created</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Month and year of initial creation</td>
      <td style="padding: 12px; background-color: #F5F7FA; border: 2px solid #D0D4D9; color: #1a1a1a; font-family: monospace;">February 2026</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Last modified</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Date of last edit (DD/MM/YYYY)</td>
      <td style="padding: 12px; background-color: #F5F7FA; border: 2px solid #D0D4D9; color: #1a1a1a; font-family: monospace;">11/02/2026</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Last reviewed by</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Name of person who last reviewed for accuracy</td>
      <td style="padding: 12px; background-color: #F5F7FA; border: 2px solid #D0D4D9; color: #1a1a1a; font-family: monospace;">Andrew Wood</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Next review due</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Scheduled review date (DD/MM/YYYY)</td>
      <td style="padding: 12px; background-color: #F5F7FA; border: 2px solid #D0D4D9; color: #1a1a1a; font-family: monospace;">11/08/2026</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Maintained by</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Team or individual responsible for updates</td>
      <td style="padding: 12px; background-color: #F5F7FA; border: 2px solid #D0D4D9; color: #1a1a1a; font-family: monospace;">Cloud Platform Team</td>
    </tr>
  </table>
</div>

**Review Schedule:**
- **Technical guides** - Review every 6 months
- **Service offerings** - Review every 3 months
- **Architecture documentation** - Review every 6 months
- **Operational procedures** - Review every 3 months
- **FAQ/Knowledge base** - Review quarterly

---

### 3. Consistent Formatting

**Use structured headings:**
```markdown
# H1 - Page Title
## H2 - Major Sections
### H3 - Subsections
```

**Use emojis for visual hierarchy:**
- 🎯 Purpose/Overview
- 📋 Scope/Requirements
- ✅ In Scope
- ❌ Out of Scope
- 🔄 Process/Workflow
- 💰 Pricing
- 📚 Related Resources
- 📞 Contact
- 📄 Page Information

**Code blocks:**
```powershell
# Use language-specific syntax highlighting
Get-AzResourceGroup -Name "rg-example"
```

**Links:**
- Internal: `[Link Text](Relative/Path)`
- External: `[Link Text](https://example.com)`

---

## 🖼️ Image Management

### Image Guidelines

1. **Only upload images that are actively referenced** in wiki pages
2. **Use descriptive filenames:** `fabric-accelerator-architecture.png` NOT `image1.png`
3. **Optimize images** before uploading (< 500KB where possible)
4. **Store in `.attachments` folder** at wiki root level
5. **Delete unused images** during quarterly reviews

### Image Reference Format

```markdown
![Alt Text Description](/.attachments/image-filename.png)
```

### Quarterly Image Cleanup

Wiki champions should:
1. List all images in `.attachments` folder
2. Search wiki for image references
3. Delete unreferenced images
4. Update image inventory

---

## 👥 Wiki Champions Program

### Responsibilities

Each team should appoint **Wiki Champions** who are responsible for:

**Monthly:**
- ✅ Review AI-generated content notices and remove when validated
- ✅ Update "Last modified" dates on edited pages
- ✅ Ensure new pages follow structure standards

**Quarterly:**
- ✅ Conduct scheduled content reviews for their team's pages
- ✅ Clean up unused images in `.attachments`
- ✅ Update "Next review due" dates
- ✅ Validate links are still active
- ✅ Archive or update outdated content

**Annually:**
- ✅ Review overall wiki structure and navigation
- ✅ Identify gaps in documentation
- ✅ Propose improvements to wiki standards

### Current Wiki Champions

<div style="width: 100%; max-width: 800px; margin: 20px auto;">
  <table style="width: 100%; border-collapse: collapse;">
    <tr style="background-color: #1B3A52;">
      <th style="padding: 12px; border: 2px solid #1B3A52; text-align: left; color: #ffffff; font-weight: bold;">Team</th>
      <th style="padding: 12px; border: 2px solid #1B3A52; text-align: left; color: #ffffff; font-weight: bold;">Champion</th>
      <th style="padding: 12px; border: 2px solid #1B3A52; text-align: left; color: #ffffff; font-weight: bold;">Backup</th>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Cloud Platform Team</td>
      <td style="padding: 12px; background-color: #F5F7FA; border: 2px solid #D0D4D9; color: #1a1a1a;">Andrew Wood</td>
      <td style="padding: 12px; background-color: #F5F7FA; border: 2px solid #D0D4D9; color: #1a1a1a;">Peter West</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-style: italic;">[Add other teams]</td>
      <td style="padding: 12px; background-color: #fffef0; border: 2px solid #D0D4D9; color: #666666; font-style: italic;">[TBD]</td>
      <td style="padding: 12px; background-color: #fffef0; border: 2px solid #D0D4D9; color: #666666; font-style: italic;">[TBD]</td>
    </tr>
  </table>
</div>

---

## 📝 Content Creation Checklist

Before publishing a new wiki page, ensure:

- [ ] Page follows the standard structure (title, hero banner, description, sections, footer)
- [ ] Hero banner is included with appropriate gradient for the section
- [ ] AI-generated content notice is included (if applicable)
- [ ] Page footer is complete with all required fields
- [ ] Next review date is scheduled
- [ ] Images are referenced correctly and uploaded to `.attachments`
- [ ] Links are tested and working
- [ ] Code examples are tested and accurate
- [ ] Spelling and grammar are correct
- [ ] Content is accessible (clear language, logical structure)

---

## 🔗 Document Storage Best Practices

### When to Use Wiki vs. SharePoint/Teams

<div style="width: 100%; max-width: 1200px; margin: 20px auto;">
  <table style="width: 100%; border-collapse: collapse;">
    <tr style="background-color: #1B3A52;">
      <th style="padding: 12px; border: 2px solid #1B3A52; text-align: left; color: #ffffff; font-weight: bold;">Content Type</th>
      <th style="padding: 12px; border: 2px solid #1B3A52; text-align: center; color: #ffffff; font-weight: bold;">Storage Location</th>
      <th style="padding: 12px; border: 2px solid #1B3A52; text-align: left; color: #ffffff; font-weight: bold;">Reasoning</th>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Technical guides</td>
      <td style="padding: 12px; background-color: #e1ffe5; border: 2px solid #D0D4D9; color: #1a1a1a; text-align: center; font-weight: bold;">✅ Wiki</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Searchable, versionable, collaborative</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Architecture diagrams</td>
      <td style="padding: 12px; background-color: #e1ffe5; border: 2px solid #D0D4D9; color: #1a1a1a; text-align: center; font-weight: bold;">✅ Wiki (as .png)</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Visual reference, embedded in docs</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Process documentation</td>
      <td style="padding: 12px; background-color: #e1ffe5; border: 2px solid #D0D4D9; color: #1a1a1a; text-align: center; font-weight: bold;">✅ Wiki</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Easy to update, accessible</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Meeting notes</td>
      <td style="padding: 12px; background-color: #ffe1e1; border: 2px solid #D0D4D9; color: #1a1a1a; text-align: center; font-weight: bold;">❌ SharePoint/Teams</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Temporary, collaborative</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Project plans</td>
      <td style="padding: 12px; background-color: #ffe1e1; border: 2px solid #D0D4D9; color: #1a1a1a; text-align: center; font-weight: bold;">❌ SharePoint/Teams</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Project-specific, may contain sensitive data</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Client documents</td>
      <td style="padding: 12px; background-color: #ffe1e1; border: 2px solid #D0D4D9; color: #1a1a1a; text-align: center; font-weight: bold;">❌ SharePoint/Teams</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Access control, compliance</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Templates (.docx, .xlsx)</td>
      <td style="padding: 12px; background-color: #ffe1e1; border: 2px solid #D0D4D9; color: #1a1a1a; text-align: center; font-weight: bold;">❌ SharePoint/Teams</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Binary files, download required</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Training materials</td>
      <td style="padding: 12px; background-color: #ffe1e1; border: 2px solid #D0D4D9; color: #1a1a1a; text-align: center; font-weight: bold;">❌ SharePoint/Teams</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Large files, video content</td>
    </tr>
    <tr>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a; font-weight: bold;">Policies & procedures</td>
      <td style="padding: 12px; background-color: #fff4e1; border: 2px solid #D0D4D9; color: #1a1a1a; text-align: center; font-weight: bold;">✅ Wiki (summary)<br>❌ SharePoint (full)</td>
      <td style="padding: 12px; background-color: #ffffff; border: 2px solid #D0D4D9; color: #1a1a1a;">Wiki for quick reference, SharePoint for official record</td>
    </tr>
  </table>
</div>

### Linking to SharePoint Documents

When referencing documents stored in SharePoint/Teams:

```markdown
For the full design document, see:
**[Platform Landing Zone Design Document](https://simpsonassociates.sharepoint.com/...)**
*(Requires SharePoint access)*
```

---

## 🔄 Review and Update Process

### Content Review Workflow

1. **Scheduled Review Trigger**
   - Wiki champion manually checks "Next review due" dates (Azure DevOps Wiki does not have built-in notifications)
   - Consider setting calendar reminders for key pages
   - Team members can flag outdated content at any time
   
2. **Review Checklist**
   - [ ] Technical accuracy validated
   - [ ] Links tested and working
   - [ ] Code examples still valid
   - [ ] Pricing/offering details current
   - [ ] Screenshots/diagrams up to date
   - [ ] AI-generated content reviewed (remove notice if validated)
   
3. **Update Footer**
   - Update "Last modified" date
   - Update "Last reviewed by" name
   - Set new "Next review due" date
   
4. **Document Changes**
   - Use git commit messages to describe significant changes
   - Consider keeping a "Revision History" section for major updates

---

## 🚨 Content Governance

### Quality Standards

**All wiki content must be:**
- ✅ **Accurate** - Technically correct and validated
- ✅ **Current** - Reflects latest practices and tools
- ✅ **Clear** - Written in plain language, well-structured
- ✅ **Consistent** - Follows wiki formatting standards
- ✅ **Accessible** - Available to appropriate audience
- ✅ **Maintainable** - Has clear ownership and review schedule

### Deprecation Process

When content becomes outdated:

1. Add a deprecation notice at the top:
```markdown
> ⚠️ **DEPRECATED**  
> This content is no longer maintained. For current information, see [New Page](link).
```

2. Update the footer with deprecation date
3. After 6 months, archive or delete deprecated pages
4. Update all links pointing to deprecated content

---

## 🛠️ Tools and Extensions

### Recommended VS Code Extensions

- **Markdown All in One** - Formatting, shortcuts, preview
- **markdownlint** - Linting and style checking
- **Markdown Preview Enhanced** - Better preview with diagrams
- **Code Spell Checker** - Catch typos

### Markdown Formatting Tools

- **Tables Generator:** https://www.tablesgenerator.com/markdown_tables
- **Emoji Lookup:** https://emojipedia.org/
- **Mermaid Diagrams:** https://mermaid.live/ *(Note: Not supported in Azure DevOps Wiki)*

---

## 📞 Questions and Support

### Wiki Governance Team

For questions about wiki standards, structure, or governance:

- **Andrew Wood** - Wiki Lead, Cloud Platform Team
- **Peter West** - Wiki Champion, Cloud Platform Team

> 💡 **Interested in becoming a Wiki Champion?** We welcome volunteers from all teams! Contact Andrew Wood or Peter West to learn more about the role.

### Suggesting Improvements

Have ideas for improving the wiki? Submit suggestions via:
- Team meetings
- Direct message to wiki champions
- Pull request to this guidelines page

---

## 📄 Page Information

**Page created:** February 2026  
**Last modified:** 11/02/2026  
**Last reviewed by:** Andrew Wood  
**Next review due:** 11/05/2026  
**Maintained by:** Cloud Platform Team
