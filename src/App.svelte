<script>
    let accounts = [
        {
            title: "",
            username: "",
            password: "",
        },
    ];

    function add(title, username, password) {
        accounts = [
            ...accounts,
            {
                title,
                username,
                password,
            },
        ];
    }

    function update(index, title, username, password) {
        accounts[index] = {
            title,
            username,
            password,
        };
    }
</script>

<style>
    h1 {
        color: #0066ff;
    }
</style>

<div>
    {#each accounts as account}
        <h1>Judul : {account.title}</h1>
        <h3>Username : {account.username}</h3>
        <h3>Password : {account.password}</h3>
    {/each}

    <button
        on:click={() => add('Twitter', 'twituser', '12233445566666')}>Add</button>

    <button
        on:click={() => update(0, 'Facebook', 'faceuser', '9182738273')}>Update</button>
</div>
