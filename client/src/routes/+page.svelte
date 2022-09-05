<script lang="ts">

    function OAuthGit()
    {
        window.location.href = "http://localhost:8000/auth/redirect";
    }
</script>


<div class="container-fluid">
    <div class="row justify-content-center" style="margin-top: 15%">
        <div class="col-5">
            <div class="card">
                <div class="card-header">
                    Login
                </div>
                <div class="card-body">
                    <input class="form-control" type="text" placeholder="Username">
                    <input type="password" class="form-control" placeholder="Password">
                    <button class="btn btn-primary" type="button" on:click={() => alert("Test")}>
                        Login
                    </button>
                    <img src="https://github.com/fluidicon.png" alt="github" height="40px" width="40px" style="border: 2px solid blue" on:click={() => OAuthGit()}>
                </div>
            </div>
        </div>
    </div>
</div>

<style>
    input {
        margin-bottom: 10px;
    }
</style>
