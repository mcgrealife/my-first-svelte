<script src='svelte.js'>
    import 

    let items = [
        {
        title: "Wow svelete is easy",
        faq: "It makes the most sense to my brain",
        img: "https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/120/apple/285/keycap-digit-zero_30-fe0f-20e3.png",
    },
    {
        title: "It reminds me of Swift, my favorite so far",
        faq: "The binding syntax is intuitive",
        img: "https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/120/apple/285/keycap-digit-one_31-fe0f-20e3.png",
    },
    {
        title: "Beginner friendly",
        faq: "It feels like HTML/CSS/JS, but with the super power of referencing {variables}",
        img: "https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/120/apple/285/keycap-digit-two_32-fe0f-20e3.png",
    }
    ];
</script>



<h2>Svelete Test</h2>


{#each items as i}
    <details>
        <summary> {i.title}</summary>
            <p>{i.faq}</p>
            <img src={i.img} alt="placeholder">
    </details>
{/each}


<style>
    h2 {
        color: red;
        font-family: Roboto;
    }
summary {
    color: purple;
    font-weight: Bold;
    font-family: Open Sans;
}
p {
    color: seagreen;
    font-family: Arial, Helvetica, sans-serif;

}
</style>