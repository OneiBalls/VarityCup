<script lang="ts">
    const teams = [{
        id: 1,
        name: "Girly Pops",
        icon: "teams/GirlyPops.png",
        iconAlt: "AGTN",
        score: 12345,
        members: [{
            name: "A Great Member",
            icon: "eventlogo.png",
            channel: "https://example.com",
        },{
            name: "A Great Member",
            icon: "eventlogo.png",
            channel: "https://example.com",
        },{
            name: "A Great Member",
            icon: "eventlogo.png",
            channel: "https://example.com",
        },{
            name: "A Great Member",
            icon: "eventlogo.png",
            channel: "https://example.com",
        }]
    },
    {
        id: 2,
        name: "A Great Team Name",
        icon: "eventlogo.png",
        iconAlt: "AGTN",
        score: 12345,
        members: [{
            name: "A Great Member",
            icon: "eventlogo.png",
            channel: "https://example.com",
        },{
            name: "A Great Member",
            icon: "eventlogo.png",
            channel: "https://example.com",
        },{
            name: "A Great Member",
            icon: "eventlogo.png",
            channel: "https://example.com",
        },{
            name: "A Great Member",
            icon: "eventlogo.png",
            channel: "https://example.com",
        }]
    }];

</script>

<main class="p-4 flex flex-col items-center lg:justify-center lg:flex-row gap-4">
    <section class="grid gap-4 max-w-100">
        <ul class="menu menu-horizontal bg-base-200 w-full">
            <li>
                <details open>
                    <!-- Load this from DB, can be removed if this is only one-time -->
                    <summary>Week 1</summary>
                </details>
            </li>
            <li>
                <details open>
                    <!-- Mandatory, load from db -->
                    <summary>Marvel Rivals</summary>
                </details>
            </li>
        </ul>

        <ul class="rounded-sm flex flex-col gap-2">
            {#each teams as team (team.id)}
                <li class="bg-base-200 flex flex-row items-center gap-2 py-1">
                    <div class="w-10 text-center">
                        <h6>{team.id}</h6>
                    </div>
                    <img class="size-6 sm:size-8" src={team.icon} alt={team.iconAlt}>
                    <div class="w-34">
                        <h2 class="font-display text-sm">{team.name}</h2>
                        <p>{team.score}</p>
                    </div>
                    <div class="flex gap-2 pr-2 flex-1">
                        {#each team.members as member}
                            <a target="_blank" href={member.channel}>
                                <img class="size-6 sm:size-8" src={member.icon} alt={member.name}>
                            </a>
                        {/each}
                    </div>
                </li>
            {/each}
        </ul>
    </section>
    <section class="bg-base-200 max-w-100 lg:w-100 p-2 rounded-sm flex flex-col gap-2">
        <h2 class="font-display text-xl">Week 1: Marvel Rivals</h2>
        <div class="grid grid-cols-3 justify-items-center" >
            <p>1</p>
            <p>vs</p>
            <p>1</p>
        </div>
    </section>
</main>