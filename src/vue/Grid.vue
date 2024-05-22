<template>
    <div class="grid-container">
        <div class="grid-item">Item 1</div>
        <div class="grid-item">Item 2</div>
        <div class="grid-item">Item 3</div>
        <div class="grid-item">Item 4</div>
        <div class="grid-item">Item 5</div>
        <div class="grid-item span-3">Item 6</div>
        <div class="grid-item span-3">Item 7</div>
        <div class="grid-item">Item 8</div>
        <div class="grid-item">Item 9</div>
    </div>
</template>

<script>
export default {
    name: 'GridComponent'
}
</script>

<style scoped>
.grid-container {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: repeat(3, auto);
    gap: 10px;
}

.grid-item {
    background-color: #f4f4f4;
    border: 1px solid #ccc;
    padding: 20px;
    text-align: center;
}

.grid-item.span-3 {
    grid-column: span 3;
}
</style>