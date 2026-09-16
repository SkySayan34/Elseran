<%*
const title = tp.file.title;
const displayName = await tp.system.prompt("Nom affiché sur le calendrier (laisser vide pour utiliser le nom du fichier)");
let output = "";

const frontmatterName = displayName ? `\nfc-display-name: "${displayName}"` : "";

if (title.includes("_")) {
  const range = title.split("_");
  const start = range[0].split("-");
  const end = range[1].split("-");
  output = `---
fc-date:
  day: ${parseInt(start[0])}
  month: ${parseInt(start[1])}
  year: ${parseInt(start[2])}
fc-end:
  day: ${parseInt(end[0])}
  month: ${parseInt(end[1])}
  year: ${parseInt(end[2])}${frontmatterName}
---

## Notes liées à cette période

\`\`\`dataview
LIST
FROM ""
WHERE contains(file.outlinks, this.file.link)
\`\`\``;
} else {
  const parts = title.split("-");
  output = `---
fc-date:
  day: ${parseInt(parts[0])}
  month: ${parseInt(parts[1])}
  year: ${parseInt(parts[2])}${frontmatterName}
---

## Notes liées à cette date

\`\`\`dataview
LIST
FROM ""
WHERE contains(file.outlinks, this.file.link)
\`\`\``

;
}

tR += output;
-%>