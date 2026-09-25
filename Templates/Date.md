<%*
const title = tp.file.title;
const displayName = await tp.system.prompt("Nom affiché sur le calendrier (vide = nom du fichier)");
const yearInput = await tp.system.prompt("Année (vide = récurrent chaque année)");

let output = "";

const frontmatterName = displayName ? `\nfc-display-name: "${displayName}"` : "";
const yearLine = yearInput ? `\n  year: ${parseInt(yearInput)}` : "";

if (title.includes("_")) {
  const range = title.split("_");
  const start = range[0].split("-");
  const end = range[1].split("-");
  output = `---
fc-date:
  day: ${parseInt(start[0])}
  month: ${parseInt(start[1])}${yearLine}
fc-end:
  day: ${parseInt(end[0])}
  month: ${parseInt(end[1])}${yearLine}${frontmatterName}
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
  month: ${parseInt(parts[1])}${yearLine}
---

## Notes liées à cette date

\`\`\`dataview
LIST
FROM ""
WHERE contains(file.outlinks, this.file.link)
\`\`\``;
}

tR += output;
-%>