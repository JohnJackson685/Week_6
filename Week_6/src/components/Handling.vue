<template>

    <p>Enter Email</p>
    <div id="email">
    <input type = 'email' v-model="email" placeholder="Enter email"/>
    <p>Email is: {{email}}</p>
    <p>Enter Age</p>
    <input type = 'text' v-model="age" placeholder="Enter age"/>
    <p>Age is: {{age}}</p>
    </div>
    <p>--------------------------------</p>
    <div>
    <p>Pick a name:</p>

    <label for="Jack">Jack</label>
    <input type="checkbox" value="Jack" v-model="name">

    <label for="Jack">Rob</label>
    <input type="checkbox" value="Rob"  v-model="name">

    <label for="Jack">George</label>
    <input type="checkbox" value="George" v-model="name">
    <p>{{name}}</p>
</div>
<p>--------------------------------</p>

<div>
    <p>Select favourite fruit:</p>
    <select v-model="selected" multiple>
        <option>Apple</option>
        <option>Banana</option>
        <option>Mango</option>
    </select>
<br>
<span>Selected: {{ selected }}</span>

</div>
</template>

<script>
export default{
    data() {
        return {
            email: '',
            age: '',
            name: [],
            selected: ''
        }
    }
}
</script>

<style>
</style>