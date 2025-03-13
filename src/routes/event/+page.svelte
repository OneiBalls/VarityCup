<main class="p-4">
    <section class="grid gap-4 w-">
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

        <table class="table bg-base-200 max-w-full">
            <thead>
                <tr>
                    <th>Ranking</th>
                    <th>Team</th>
                    <th>Members</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <th>1</th>
                    <th class="flex flex-row gap-4 items-center">
                        <img class="size-10" alt="Icon" src="eventlogo.png">
                        <div class="flex flex-col">
                            <h1 class="font-display">A Great Team Name</h1>
                            <p>12345</p>
                        </div>
                    </th>

                    <!-- This should be from the DB-->
                    <th class="flex flex-row items-center gap-4">
                        <a target="_blank" href="https://example.com">
                            <div class="bg-base-300 size-10 rounded-full">
                                <img class="aspect-square" alt="Member name" src="eventlogo.png">
                            </div>
                        </a>
                        <a target="_blank" href="https://example.com">
                            <div class="bg-base-300 size-10 rounded-full">
                                <img class="aspect-square" alt="Member name" src="eventlogo.png">
                            </div>
                        </a>
                        <a target="_blank" href="https://example.com">
                            <div class="bg-base-300 size-10 rounded-full">
                                <img class="aspect-square" alt="Member name" src="eventlogo.png">
                            </div>
                        </a>
                        <a target="_blank" href="https://example.com">
                            <div class="bg-base-300 size-10 rounded-full">
                                <img class="aspect-square" alt="Member name" src="eventlogo.png">
                            </div>
                        </a>
                    </th>
                </tr>
            </tbody>
        </table>
    </section>
</main>