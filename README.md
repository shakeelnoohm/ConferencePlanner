# Conference Expense Planner

A React + Redux Toolkit web app for planning and budgeting corporate conference events.

## Features

- **Venue Selection** — Browse and add conference rooms (Conference Room, Auditorium Hall, Presentation Room, Large/Small Meeting Rooms) with quantity controls. The Auditorium Hall is capped at a maximum of 3 bookings.
- **Add-ons Selection** — Select AV equipment (Projectors, Speakers, Microphones, Whiteboards, Signage) with individual quantity controls.
- **Meals Selection** — Choose meals (Breakfast, High Tea, Lunch, Dinner) with per-person cost calculation based on the number of attendees.
- **Live Cost Summary** — Toggle a detailed breakdown view showing all selected items, unit costs, quantities, subtotals, and a grand total.

## Tech Stack

- [React 18](https://react.dev/) — UI framework
- [Redux Toolkit](https://redux-toolkit.js.org/) — State management (`venueSlice`, `avSlice`, `mealsSlice`)
- [Vite](https://vitejs.dev/) — Build tool and dev server

## Getting Started

### Prerequisites

- Node.js ≥ 18

### Install & Run

```bash
npm install
npm run dev
```

The app will be available at `http://localhost:5173`.

### Build for Production

```bash
npm run build
npm run preview
```

## Project Structure

```
src/
├── main.jsx              # Entry point, Redux Provider
├── App.jsx               # Landing page + ConferenceEvent mount
├── ConferenceEvent.jsx   # Main planner UI
├── TotalCost.jsx         # Cost summary component
├── AboutUs.jsx           # About section
├── store.js              # Redux store
├── venueSlice.js         # Venue state & reducers
├── avSlice.js            # AV add-ons state & reducers
└── mealsSlice.js         # Meals state & reducers
```

## License

[MIT](LICENSE)