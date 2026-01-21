<%*
const today = tp.date.now("YYYY-MM-DD");
const wday = tp.date.now("dddd");
const yesterday = tp.date.yesterday("YYYY-MM-DD");
const tomorrow = tp.date.tomorrow("YYYY-MM-DD");;
// Renames the current file to the current date in 'YYYY-MM-DD' format
await tp.file.rename(tp.date.now("YYYY-MM-DD"));
%>
---
createdAt: <% tp.file.creation_date() %>
--- 
tags: 
# # 📅 <% today %>  <% wday %>

[[<% yesterday %>]] [[<% tomorrow %>]]
## ##🌤️ Morning Reflection
- Mood: 
- Energy: 
- Focus: 

## ## ✅ Top 3 Priorities
1. <% tp.file.cursor() %>
2. 
3. 

## ## 📓 Notes and TaskNotes
- 

## ## 📊 End of Day Review
- Wins: 
- Challenges: 
- Lessons Learned: 
