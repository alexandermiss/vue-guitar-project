<template>
    <div>
        <h1>Guitar!</h1>
        <vc-chord-diagram :setup="noteAm" />
    </div>
</template>

<script>
    import VcChordDiagram from 'vc-chord-diagram';
    import './node_modules/vc-chord-diagram/dist/lib/vc-chord-diagram.min.css'

    export default {
        components: {
            VcChordDiagram
        },
        data(){
            return {
                noteAm : {
                    startAt: 1,
                    tuning: ['E', 'A', 'D', 'G', 'B', 'E'],
                    strings: [{
                        fret: 0,
                        finger: 'x'
                    }, {
                        fret: 0,
                        finger: 0
                    }, {
                        fret: 2,
                        finger: 3
                    }, {
                        fret: 2,
                        finger: 2
                    }, {
                        fret: 1,
                        finger: 1
                    }, {
                        fret: 0,
                        finger: 0
                    }]
                }
            };
        }
    }
</script>