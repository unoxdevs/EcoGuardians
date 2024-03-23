<script>
    let cardInfos = [
        {
            title: "Why Nature Counts: Your link to the wilderness",
            description: "We connect you to the wild through your fingertips, with access to live feeds, interactive tours, and conservation efforts. Nature’s Heart – your pass to Planet Earth.",
            writer: "Oliver Woods"
        },
        {
            title: "Join the Force: Conserving nature, one click at a time.",
            description: "Join our vibrant community of Earth warriors. Together, we can make a difference. You’re the hero Nature needs.",
            writer: "Emma Green"
        },
        {
            title: "The Great Outdoors: Your next adventure awaits",
            description: "We’re your guide to the great outdoors. From the Amazon to the Arctic, we’ve got you covered. Get ready to explore.",
            writer: "Oliver Woods"
        }
    ]
</script>

<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-3 px-5 md:px-7 lg:px-24 py-10">
    {#each cardInfos as cardInfo}
        <div class="bg-[#DAE1D0] rounded-lg overflow-hidden">
            <img src="https://source.unsplash.com/1600x900/?nature,water,tree,forest,sky" alt="Nature" class="w-full h-64 object-cover">
            <div class="p-4">
                <span class="text-xs my-2">{cardInfo.writer}</span>
                <h1 class="text-xl font-bold">{cardInfo.title}</h1>
                <p class="text-sm py-2">{cardInfo.description}</p>
            </div>
        </div>
    {/each}
</div>