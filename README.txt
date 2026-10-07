HOW TO RUN
1. In this folder run:  python -m http.server 8000   (or VS Code "Live Server", or "npx serve")
2. Open http://localhost:8000/login.html     Demo login: any ID, password survey123
   GPS and camera need localhost or HTTPS. For phones, host the folder on Netlify / GitHub Pages.

FLOW
Home -> your details (name, mobile, residential location) -> choose role: Area DC (Forms 1-7) or People DC (Form 8) -> register area (State, District, Taluka/Division, Village) -> fill forms.
Top-right button switches English / Telugu (data is always stored in English).

WHERE TO CHANGE THINGS
login.html                     login screen, demo password
index.html                     role choice, area registration, dashboard, sync, export
form1.html ... form8.html      field lists (edit the sections arrays)
js/app.js                      shared engine (validation, tables, auto-calc, GPS, camera, drafts)
js/data.js                     State -> districts list (Telangana and Andhra Pradesh)
js/te.js                       Telugu translations (English text -> Telugu)
css/style.css                  colours and layout
