<template>
    <div>
        <p>the time</p>
        <p>the clicks = {{$store.state.counter}}</p>
        <button @click="$store.commit('increment')">Add</button>
        <h1>The Time {{$store.state.time}}</h1>
    </div>
</template>
<script>


export default {
    props:{
        time:Number,
    }
}
</script>
