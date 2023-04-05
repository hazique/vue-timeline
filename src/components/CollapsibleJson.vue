<script>
import * as renderjson from 'renderjson'


export default {
    props: {
        data: {
            type: Object,
            // Object or array defaults must be returned from
            // a factory function. The function receives the raw
            // props received by the component as the argument.
            default(rawProps) {
                return {}
            }
        },
        id: String
    },
    data() {
        return {
        }
    },

    mounted() {
        const parent = document.getElementById(this.id)
        const el = renderjson(this.data)
        parent.appendChild(el)
    }
}

</script>

<template>
    <v-timeline-item>
        <div style="width: 50px;" :id=id>
            <div>{{ id }}</div>
        </div>
    </v-timeline-item>
</template>

<style>
/* #container {
  text-shadow: none;
  background: #303030;
  padding: 1em;
} */

/* .v-timeline-divider{
  width: 110%  !important;
} */

.renderjson a {
    text-decoration: none;
}

.renderjson .disclosure {
    color: crimson;
    font-size: 150%;
}

.renderjson .syntax {
    color: grey;
}

.renderjson .string {
    color: red;
}

.renderjson .number {
    color: cyan;
}

.renderjson .boolean {
    color: plum;
}

.renderjson .key {
    color: lightblue;
}

.renderjson .keyword {
    color: lightgoldenrodyellow;
}

.renderjson .object.syntax {
    color: lightseagreen;
}

.renderjson .array.syntax {
    color: lightsalmon;
}
</style>

