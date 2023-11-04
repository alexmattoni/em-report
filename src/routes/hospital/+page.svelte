<script lang="ts">
    import type { PageData } from './$types';
    import { MapLibre } from 'svelte-maplibre';

    // export let data: PageData;
</script>

<body class="container-fluid">
    <h1 class="mb-2" style="font-size: 2.5em;"> Hospital Dashboard</h1>
    <div class = "container-fluid">
        
        <h1 class="mb-2" style="font-size: 1.2em;"> Incoming Patients</h1>
        <table> 
            <!--
            <tr>
                {#each data.patients.data as patient}
                    <article>{patient.lastname, patient.firstname} </article>
                {/each}
            </tr>
            -->
        </table>
    </div>

    <!-- credit: MapLibre mapping libre Svelte wrapper -->

    <div class="container-fluid">
        <h1 class="mb-2" style="font-size: 1.2em;" > Unit Map </h1>
        <MapLibre
        style="https://basemaps.cartocdn.com/gl/positron-gl-style/style.json"
        class="relative w-full aspect-[9/16] max-h[70vh] sm:max-h-full sm:aspect-video"
        standardControls
        zoom={7}
        center={[-73.75, 42.5]}
        >
        <!--
        {#each markers as { lngLat, label, name } (label)}
            <Marker
            {lngLat}
            on:click={() => (clickedName = name)}
            class="border-gray-200 border shadow-2xl focus:outline-2 focus:outline-black w-8 h-8 bg-red-300 text-black rounded-full grid place-items-center"
            >
            <span>
                {label}
            </span>

            <Popup openOn="hover" offset={[0, -10]}>
                <div class="text-lg font-bold">{name}</div>
            </Popup>
            </Marker>
        {/each}
        -->
        </MapLibre>
    </div>
</body>