<template>
  <div class="todoapp">
      <h1 class="todoapp__title">todos</h1>

      <div class="todoapp__content">
        <header class="todoapp__header">
          <button
            data-cy="ToggleAllButton"
            type="button"
            class="todoapp__toggle-all active"
          />

          <form>
            <input
              data-cy="NewTodoField"
              type="text"
              ref={newTodoField}
              class="todoapp__new-todo"
              placeholder="What needs to be done?"
            />
          </form>
        </header>

        <section class="todoapp__main" data-cy="TodoList">
          <div data-cy="Todo" class="todo completed">
            <label class="todo__status-label">
              <input
                data-cy="TodoStatus"
                type="checkbox"
                class="todo__status"
                defaultChecked
              />
            </label>

            <span data-cy="TodoTitle" class="todo__title">HTML</span>
            <button
              type="button"
              class="todo__remove"
              data-cy="TodoDeleteButton"
            >
              ×
            </button>

            <div data-cy="TodoLoader" class="modal overlay">
              <div class="modal-background has-background-white-ter" />
              <div class="loader" />
            </div>
          </div>

          <div data-cy="Todo" class="todo">
            <label class="todo__status-label">
              <input
                data-cy="TodoStatus"
                type="checkbox"
                class="todo__status"
              />
            </label>

            <span data-cy="TodoTitle" class="todo__title">CSS</span>

            <button
              type="button"
              class="todo__remove"
              data-cy="TodoDeleteButton"
            >
              ×
            </button>

            <div data-cy="TodoLoader" class="modal overlay">
              <div class="modal-background has-background-white-ter" />
              <div class="loader" />
            </div>
          </div>

          <div data-cy="Todo" class="todo">
            <label class="todo__status-label">
              <input
                data-cy="TodoStatus"
                type="checkbox"
                class="todo__status"
              />
            </label>

            <form>
              <input
                data-cy="TodoTitleField"
                type="text"
                class="todo__title-field"
                placeholder="Empty todo will be deleted"
                defaultValue="JS"
              />
            </form>

            <div data-cy="TodoLoader" class="modal overlay">
              <div class="modal-background has-background-white-ter" />
              <div class="loader" />
            </div>
          </div>

          <div data-cy="Todo" class="todo">
            <label class="todo__status-label">
              <input
                data-cy="TodoStatus"
                type="checkbox"
                class="todo__status"
              />
            </label>

            <span data-cy="TodoTitle" class="todo__title">React</span>
            <button
              type="button"
              class="todo__remove"
              data-cy="TodoDeleteButton"
            >
              ×
            </button>

            <div data-cy="TodoLoader" class="modal overlay">
              <div class="modal-background has-background-white-ter" />
              <div class="loader" />
            </div>
          </div>

          <div data-cy="Todo" class="todo">
            <label class="todo__status-label">
              <input
                data-cy="TodoStatus"
                type="checkbox"
                class="todo__status"
              />
            </label>

            <span data-cy="TodoTitle" class="todo__title">Redux</span>
            <button
              type="button"
              class="todo__remove"
              data-cy="TodoDeleteButton"
            >
              ×
            </button>

            <div data-cy="TodoLoader" class="modal overlay is-active">
              <div class="modal-background has-background-white-ter" />
              <div class="loader" />
            </div>
          </div>
        </section>

        <footer class="todoapp__footer" data-cy="Footer">
          <span class="todo-count" data-cy="todosCounter">
            4 items left
          </span>

          <nav class="filter" data-cy="Filter">
            <a
              data-cy="FilterLinkAll"
              href="#/"
              class="filter__link selected"
            >
              All
            </a>

            <a
              data-cy="FilterLinkActive"
              href="#/active"
              class="filter__link"
            >
              Active
            </a>
            <a
              data-cy="FilterLinkCompleted"
              href="#/completed"
              class="filter__link"
            >
              Completed
            </a>
          </nav>

          <button
            data-cy="ClearCompletedButton"
            type="button"
            class="todoapp__clear-completed"
          >
            Clear completed
          </button>
        </footer>
      </div>

    </div>
</template>

