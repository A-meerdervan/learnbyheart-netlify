<script>
    // I think these export values are ones that can be assigned to from outside this component
    // They can be set when creating the instance
    export let points;
    export let totalAsked;
    export let set_Length;
    let procent = 0;
    let questionsLearned = 0;

    export function setScores(points,totalAsked){
        // console.log('GetProcent now called');
        // console.log('totalAsked: %d', totalAsked);
        if (totalAsked == 0){
            procent = 0;
        }
        else{
            procent = Math.round(points / totalAsked * 100)
        }
    }

    export function setQuestionsLearned(nrOfZeros,set_Length){
        questionsLearned = nrOfZeros;
        set_Length = set_Length;
    }

</script>

<style>
    .Points {
        position: relative;
        right: 0px;
        top: 0px;
        color: green;
    }

</style>

<div class = 'Points'>
    <h3>Facts learned: {questionsLearned} out of {set_Length} | Score: {points} out of {totalAsked} = {procent} % </h3>
</div>