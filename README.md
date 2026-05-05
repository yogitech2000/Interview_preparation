# DevOps/SRE Interview Prep Prototype

A static prototype for an interview preparation dashboard built in a single HTML file. It is designed to help review DevOps, SRE, cloud, and coding questions with category-based navigation, search, filtering, and lightweight persistence.

## Description

This prototype is a client-side web app with an interactive sidebar, expandable question cards, search filters, and local persistence using `localStorage`. It is intended as a personal prep tool and not a production-ready system.

## Key Features

- Sidebar navigation with categories and topics
- Search bar for filtering questions and answers
- Difficulty filters: All / Easy / Medium / Hard
- Reviewed and Bookmarked toggles
- Question cards with expandable answers
- Notes textarea per question
- Add new custom questions
- Import / Export question data as JSON
- Theme toggle (dark / light)
- Persistent state using `localStorage`
- Organization section supports:
  - Add new company entries
  - Delete company entries

## How to Use

1. Open `interview_prep_Final.html` in a browser.
2. Use the sidebar to navigate categories and topics.
3. Search questions using the top toolbar search input.
4. Filter by difficulty or toggle Reviewed / Bookmarked views.
5. Click a question card to expand the answer.
6. Use the `+ Add Question` button to create a new question.
7. Use Import / Export to save or load JSON data.
8. Add or delete company entries under `Organizations`.

## Persistence

The app stores data locally in the browser via `localStorage`:

- `prepkit_data`
- `prepkit_reviewed`
- `prepkit_bookmarked`
- `prepkit_notes`
- `prepkit_theme`

This means custom questions and company entries persist across page refreshes in the same browser.

## Project Structure

The application is implemented in a single HTML file with embedded:

- CSS for layout, theme, and responsive behavior
- HTML for the UI structure and modal panels
- JavaScript for state management, rendering, persistence, and interaction logic

## Extending the Prototype

If you want to extend the app, consider adding:

- A proper question editor with validation
- A full company/topic management panel instead of prompt-based input
- Drag-and-drop reordering for topics and questions
- Export/import version history or backup support
- Search highlighting improvements using regex-safe matching

## Notes

- This is a prototype, so the focus is on functionality over formal architecture.
- All logic is currently inside `interview_prep_Final.html`.
- The app is self-contained and requires no server.

## Open in Browser

Simply open `interview_prep_Final.html` in any modern browser to run the prototype.
