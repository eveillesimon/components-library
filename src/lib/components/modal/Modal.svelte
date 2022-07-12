<script>
    export let id;
    export let opened = true;

    function close() {
        opened = false;
    }
</script>

<div id="{id}"
     class="fixed z-50 left-0 top-0 w-screen h-screen overflow-auto bg-black/75 "
     class:hidden={!opened}
>
    <div class="bg-white">
        <button on:click={close}>Close Modal</button>
    </div>
</div>
