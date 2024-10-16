<template>
    <h3>Table</h3>
    <table>
        <thead>
            <tr>
                <th>Sport</th>
                <th>Skill Level</th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="(skill, sport) in sportSkills" :key="sport">
                <td>{{ sport }}</td>
                <td>{{ skill }}</td>
            </tr>
        </tbody>
    </table>
</template>

<script setup>
const props = defineProps({
    sportSkills: {
        type: Object,
        required: true
    }
})
</script>