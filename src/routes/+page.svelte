<script>
    let name="Maina";

    import Counter from "../lib/Counter.svelte";
    const props={
        maxCount:10,
        initialCount:5
    };
</script>

<Counter {...props} x="y"/> 
<h1>Hello {name.toUpperCase()}</h1>

<style>
    h1{
        color:darkred
    }
</style>