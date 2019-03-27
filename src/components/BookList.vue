<template>
    <div>
        <h1>{{ title }}</h1>
        <ul>
            <li v-for="book in books">{{book.title}}: {{book.author}}</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'Booklist',
    data() {
        return {
            title: 'All Books',
            books: [
                {title: 'test 1', author: 'test 1'},
                {title: 'test 2', author: 'test 2'}
            ]
        }
    }
}
</script>

<style>
h1, h2 {
    font-weight: normal
}
ul {
    list-style-type: none;
    padding: 0;
}
li {
    display: block;
    margin: 0 10px;
}
</style>
