# Polya for ChatGPT and Claude

Polya is a course-aware study tutor. This plugin brings the courses you've added to Polya into ChatGPT and Claude: the AI can see the study mode you chose for each course (from hints only to full worked solutions) and search your course materials so its explanations cite what your class actually covers.

## What you need

A Polya account at [askpolya.com](https://askpolya.com) with at least one course added. You sign in to Polya when you connect the plugin.

## Tools

| Tool | What it does |
|---|---|
| `list_my_courses` | Lists the courses you've added to Polya. |
| `get_course_rules` | Returns a course's study mode: what kind of help you've chosen, and what's off the table. |
| `search_course_materials` | Searches a course's readings, slides, pages and lecture transcripts and returns cited passages. Practice mode never returns answer keys. |

All three tools only read. Nothing in Polya or your school's systems is changed.

## Install

- **Claude (web, desktop, mobile):** Customize > Connectors > Add custom connector, and enter `https://askpolya.com/mcp`.
- **Claude Code:** `claude plugin marketplace add hqscope/polya-plugin`, then `claude plugin install polya@polya`.
- **ChatGPT:** find Polya in the plugin directory, or (developer mode) add `https://askpolya.com/mcp` as a plugin.

## Privacy

See [askpolya.com/privacy](https://askpolya.com/privacy). Support: hello@askpolya.com.
