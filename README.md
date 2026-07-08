<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CSS Grid - Areas</title>
  <style>
    .layout {
      display: grid;
      grid-template-areas:
        "header header header"
        "menu main aside"
        "footer footer footer";
      grid-template-columns: 1fr 1fr 1fr;
      grid-template-rows: auto auto auto;
      gap: 10px;
      row-gap: 10px;
    }
    .header { grid-area: header; background: lightblue; padding: 20px; text-align: center; }
    .menu   { grid-area: menu; background: lightgreen; padding: 20px; }
    .main   { grid-area: main; background: lightyellow; padding: 20px; }
    .aside  { grid-area: aside; background: lightpink; padding: 20px; }
    .footer { grid-area: footer; background: lightgray; padding: 20px; text-align: center; }
  </style>
</head>
<body>
  <h2>Web Page Layout using Grid</h2>
  <div class="layout">
    <div class="header">Header</div>
    <div class="menu">Menu</div>
    <div class="main">Main Content</div>
    <div class="aside">aside</div>
    <div class="footer">Footer</div>
  </div>
</body>
</html>
