---
id: |-
  <%* 
  const bugId = await tp.system.prompt("Bug ID เช่น BUG-001", "BUG-001");
  tR += bugId;
  %>
title: <% tp.file.title %>
date: <% tp.date.now("YYYY-MM-DD HH:mm") %>
reporter: |-
  <%* 
  const reporter = await tp.system.prompt("Reporter name", "tester-name");
  tR += reporter;
  %>
severity: |-
  <%* 
  const severity = await tp.system.suggester(
    ["low", "medium", "high", "critical"],
    ["low", "medium", "high", "critical"]
  );
  tR += severity;
  %>
status: open
consult_first: false
runner_portal_area: e.g. checkout / event-list / auth / registration
---

## Steps to Reproduce

1. 
2. 
3. 

## Expected Result

What should happen.

## Actual Result

What actually happens.

## Environment

- Device: e.g. iPhone 15 / Chrome desktop
- OS: e.g. iOS 18 / macOS 15
- Browser: e.g. Safari 18 / Chrome 124
- Runner Portal version / commit: e.g. `main` @ `abc1234`

## Screenshots

![[attachments/BUG-000-screenshot-1.png]]

## Additional Notes

Any extra context, logs, or related issues.
