# Counter & ToDos App

A simple Angular application demonstrating the use of signals, standalone components, pipes, services, and directives. It combines a counter feature with a Todo list fetched from an API.

## 🧩 Features

- Counter component using Angular signals
- Greeting component with dynamic input
- Todo list fetched from a REST API
- Custom directive to highlight completed todos
- Filter pipe for live todo searching
- Component interaction using `@input`, `@output`, and signals
- Keyboard event handling

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or higher)
- [Angular CLI](https://angular.io/cli)

### Installation

```bash
git clone https://github.com/yourusername/counter-todos-app.git
cd counter-todos-app
npm install
```

## Run the Application

```bash
ng serve
```
Visit http://localhost:4200 in your browser.

## Components overview

`CounterComponent`
- Simple signal-based counter with increment, decrement, and reset.

`GreetingComponent`
- Displays a greeting message using input() from Angular signals.
 
`TodoItemComponent`
- Represents a single Todo.
- Emits a todoToggled event on click.

`HomeComponent`
- Displays greeting and counter components.
- Logs keyboard events.

`TodosComponent`
- Fetches and displays todos.
- Includes a search input and highlights completed items.

## Services

`TodosService`
Fetches todos from: https://jsonplaceholder.typicode.com/todos

## Pipes

`FilterTodosPipe`
- Filters todos based on a search string (case-insensitive).

## Directives

`HighlightCompletedTodoDirective`
- Adds styles (strikethrough and background color) to completed todos dynamically via signals.


