<script>
    export let initialCount;
    export let maxCount;
    let count=initialCount;
    // let count1=0
    // let count2=0
    // // let string=`You have clicked ${count} times`

    // let string;
    //reactive statement
    // $:string=`You have clicked ${count} times`
    

    // $: if(count>5){
    //     console.log(`The count is ${count}`)
    // }
        // function setCount2(x){
        //     count2=x;
        // }
        // //order pf reactive statements is important
        // $: setCount2(count1);
        // $: string=`Count2 is ${count2}`

        console.log($$props,$$restProps)
    function increment1(){
        if(count===maxCount) return;
        count++
    }
    
</script>

<h1> I am Counter</h1>
<button on:click={increment1}>Click {count}</button>
<!-- <h3>{string}</h3> -->

<style>
    button{
        padding: 10px 20px;
    }
</style>