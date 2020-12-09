<template>
  <amplify-authenticator>
    <h1>TodoApp</h1>
    <v-text-field v-model="name" label="Name"></v-text-field>
    <v-text-field v-model="description" label="Description"></v-text-field>
    <v-btn @click="createTodo">Create</v-btn>
    <ul>
      <li v-for="todo in todos" :key="todo.id">
        {{ todo.name }} : {{ todo.description }}
      </li>
    </ul>
    <amplify-sign-out></amplify-sign-out>
  </amplify-authenticator>
</template>
