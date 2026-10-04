---
name: polya-course-rules
description: Use when the student asks for help with coursework, homework, a problem set, a lab, a reading or an exam topic for a class they study with Polya. Checks that course's study rules first, keeps help within them, and grounds explanations in the course's own materials.
---

# Helping with coursework inside a course's study rules

The student has added their courses to Polya. For each course they have chosen a study mode that says what kind of help they want. Treat it as the limit of your help for that course.

## Steps

1. If you don't have the course handle yet, call `list_my_courses` and pick the course the student means. Ask if it's ambiguous.
2. Call `get_course_rules` for that course before helping with its coursework.
3. Keep your help inside the rules:
   - **Open**: full answers and walkthroughs are fine when asked.
   - **Guided**: explain concepts fully, but on problems give hints, a guiding question or one step at a time. Hold back a full solution until the student has shown their own attempt in this conversation.
   - **Practice**: quiz the student. Don't state an answer before they commit to one, give at most one guided step at a time, and don't use answer keys.
   - **Review**: full worked solutions are fine, ideally followed by a related practice task.
4. When a request goes past the rules, say so plainly, quote the rule, and offer the help that is allowed. Don't lecture.
5. Use `search_course_materials` to ground explanations in the course. Cite passages by their [n] number and say where they come from (for example, "Lecture 7, pages 4 to 5").

## Notes

- The rules come from the student's settings in Polya. Don't describe them as rules set by the instructor.
- If a course shows as still loading, say its materials aren't ready yet and help in general terms within the rules.
