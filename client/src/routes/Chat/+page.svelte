<script lang="ts">
    import Message from '../../lib/components/Message.svelte';

let publicMessages = [
    {
        name: "Test",
        message: "This is a test message"
    }
];

</script>


<div class="container-fluid">
    <div class="row">
        <div class="col">
            <div class="card">
                <div class="card-header">
                    Public Chat
                </div>
                <div class="card-body">
                    {#each publicMessages as Message}
                        <Message name={Message.name} message={Message.message}/>
                    {/each}
                </div>
            </div>
        </div>
        <div class="col">
            <div class="card">
                <div class="card-header">
                    Private Chat
                </div>
                <div class="card-body">

                </div>
            </div>
        </div>
    </div>
</div>