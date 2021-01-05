<script>
    let title = "Facebook";
    let username = "siapaajalah";
    let password = "sangatRahasiaAtuh123456";
    let html_data = "<h1>Ini html data</h1>";
</script>

<style>
    h1 {
        color: #0066ff;
    }
</style>

<div>
    <h1>Judul : {title}</h1>
    <h3>Username : {username}</h3>
    <h3>Password : {password}</h3>
    <p>
        {@html html_data}
    </p>
</div>
