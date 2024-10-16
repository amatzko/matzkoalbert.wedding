<template>
    <h1>About us</h1>
    
    <div class="relationship-blurb">
        <h2>Our Story</h2>
        <p>
            Our journey together began in the vibrant landscapes of the Middle East. 
            We met while working on a project in Tel Aviv, where the Mediterranean 
            breeze carried the promise of new beginnings. Our shared experiences 
            in this culturally rich region not only brought us closer but also 
            shaped our worldview and strengthened our bond.
        </p>
        <p>
            From exploring ancient ruins in Jerusalem to savoring falafel in the 
            bustling markets of Amman, our adventures in the Middle East became 
            the foundation of our relationship. These experiences taught us the 
            value of embracing different cultures and the importance of understanding 
            and respecting diverse perspectives.
        </p>
        <p>
            As we moved forward in our careers and lives, the lessons and memories 
            from our time in the Middle East remained a cherished part of our story. 
            They continue to influence our decisions, our values, and our vision 
            for our future together.
        </p>
    </div>

    <div class="wedding-registry">
        <h2>Our Wedding Registry</h2>
        <RegistryItem
            v-for="item in registryItems"
            :key="item.id"
            :item="item"
            @update:purchased="updatePurchaseStatus"
        />
    </div>
</template>

<script setup>

const registryItems = ref([])

onMounted(async () => {
    const { data } = await useFetch('/api/registry')
    registryItems.value = data.value
})

const updatePurchaseStatus = async (itemId) => {
    const item = registryItems.value.find(item => item.id === itemId)
    if (item) {
        item.purchased = true
        await $fetch(`/api/registry/${itemId}`, {
            method: 'PUT',
            body: item
        })
    }
}
</script>

<style scoped>
.relationship-blurb {
    background-color: #1a1a1a;
    color: #ff0000;
    padding: 20px;
    border: 2px solid #ff0000;
    font-family: 'Courier New', monospace;
}

.relationship-blurb h2 {
    text-transform: uppercase;
    letter-spacing: 3px;
    text-shadow: 2px 2px #000000;
}

.relationship-blurb p {
    text-align: justify;
    line-height: 1.6;
    margin-bottom: 15px;
}

.relationship-blurb p::first-letter {
    font-size: 150%;
    font-weight: bold;
}
.wedding-registry {
    margin-top: 40px;
}
</style>

