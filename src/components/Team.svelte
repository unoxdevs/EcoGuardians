<script>
    let teamUsers = [
        {
            name: "Oliver Woods",
            role: "Head of Conservation"
        },
        {
            name: "Emma Green",
            role: "Biodiversity Chief"
        },
        {
            name: "Liam Wild",
            role: "Eco Development Head"
        }
    ]
</script>

<div class="px-24 py-20">
    <h1 class="text-2xl md:text-3xl lg:text-3xl text-center items-center">Meet The Team</h1>
    <p class="py-3 text-center items-center text-sm md:text-base lg:text-base">Our team is a thinktank of eco-warriors and nature enthusiasts, committed to making difference.</p>
    <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-3 gap-3 py-10">
        {#each teamUsers as user}
            <div class="bg-[#DAE1D0] rounded-lg overflow-hidden p-5">
                <!-- svelte-ignore a11y-img-redundant-alt -->
                <img class="w-16 rounded-full" src="https://xsgames.co/randomusers/avatar.php?g=pixel" alt="Profile Photo">
                <h1 class="mt-5">{user.name}</h1>
                <p class="text-sm py-2">{user.role}</p>
                <button class="mt-5 p-2 bg-gray-900 px-10 rounded-lg text-white text-sm"><p>Contact</p></button>
            </div>
        {/each}
    </div>
</div>
