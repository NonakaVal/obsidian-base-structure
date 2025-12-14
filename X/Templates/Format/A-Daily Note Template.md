---
created: <% tp.date.now("YYYY-MM-DD @ HH:mm") %>
tags:
  - calendar/daily
week: '[[<% tp.date.now("YYYY [Week] WW") %>]]'
---

<% tp.date.now("YYYY-MM-DD") %>’s Note

[[<% tp.date.yesterday("YYYY-MM-DD") %>|↶ Previous Day]] | [[<% tp.date.tomorrow("YYYY-MM-DD") %>|Following Day ↷]]

# Work Log #log

<%tp.file.cursor()%>

---


<%*
const folderPath = "04 Calendar & Review/Daily Notes";
if (!tp.app.vault.getAbstractFileByPathInsensitive(folderPath)) {
  await tp.app.vault.createFolder(folderPath);
}
await tp.file.move(`${folderPath}/${tp.file.title}`);
-%>

